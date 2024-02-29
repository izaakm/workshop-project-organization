---
title: Exercise -- Create a "make project" script
---

# What next ... ?

> ... any additional overhead means that something just won't get done. So if
> setting up a project isn't almost as simple as just making a new directory,
> then a lot of users will simply make new blank project directories and fill
> them up with minimal consideration to structure like they've been doing even
> though they know it leads to headaches.


# Exercise 
## Create a "make project" script

The goal:

```
$ mkprj future-nature-pub
```

1. Create directory "future-nature-pub".
1. Create your standard set of directories.
1. Create your standard set of files, e.g., README, AUTHORS.
1. Initialize the directory as a Git repository with your standard files (and directories).

# Exercise 
## Create a "make project" script

```
$ cd /lustre/isaac/scratch/USERNAME
$ mkdir -p src/make-project
$ cd src/make-project
$ nano make-project.sh
```

Add the following text to your script:

```text
#!/usr/bin/env bash
```

# Exercise

*Don't forget to save your changes!*

In Nano:

- Press <kbd>Control</kbd><kbd>o</kbd> to "write out" the file.
- Then press <kbd>Enter</kbd> to confirm.

# Exercise

```text
# Don't overwrite files, just to be safe.
set -o noclobber
```

# Exercise

```text
# Exit immediately if any command returns an error code.
set -e
```

# Exercise

```text
# Exit if no arguments were provided.
if [ $# -eq 0 ] ; then
    echo "Create a new project directory."
    echo "Usage: $0 <project>"
    exit 1
fi
```

# Exercise

```text
# The first argument passed into the script should be the name of the directory
# where you want your new project directory created.
project_dir="$1"

echo "Setting up folder structure in ${project_dir}"
```

# Exercise

```text
# Make the project directory then cd into it.
mkdir "${project_dir}"
cd "${project_dir}"

# Create directories.
mkdir data docs notebooks results src
```

# Exercise
## Create `AUTHORS` file

Use the `touch` command to create a new, empty file:

```text
touch "AUTHORS"
echo "AUTHORS file created."
```

# Exercise
## Create `.gitignore` file
 
```text
# Ignore some files.
cat <<EOF > .gitignore
tmp
EOF
```

# Exercise

```text
cat <<EOF
...
EOF
```

The **heredoc** `<<EOF` tells `cat` to "read lines of text `...` until you see the line `EOF`."


# Exercise

```text
> .gitignore
```

The right angled bracket `>` means "instead of printing the output to the
terminal (aka, `stdout`), **redirect** it to the file `.gitignore`."

# Exercise
## Create `.gitignore` file
 
Write the <u>lines</u> between `<<EOF` and `EOF` to the `.gitignore` file:

```text
# Ignore some files.
cat <<EOF > .gitignore
tmp
EOF
```

# Exercise

Create dummy files so that Git will know about these directories.

```text
# Creat dummy files.
touch data/.gitkeep
touch docs/.gitkeep
touch notebooks/.gitkeep
touch results/.gitkeep
touch src/.gitkeep
```

# Exercise
## Setup data subdirectories

Even if you don't want the files in these directories to be tracked by git, you
still want to be sure that the same directory structure exists on any/all
remotes.

```text
# Create data subdirectories.
mkdir data/anthro data/derived data/raw 

# Creat dummy files.
touch data/anthro/.gitkeep
touch data/derived/.gitkeep
touch data/raw/.gitkeep
```

# Exercise
## Ignore (almost) everything inside the data directory.

```text
cat <<EOF > data/.gitignore 
*
!.gitignore
!.gitkeep
EOF

echo "Folders created."
```

# Exercise
## Create the README file.

```text
cat <<EOF > README.md
# PROJECT TITLE

Description of your project.

## Project structure

    ${project_dir}
    ├── README.md
    ├── data       => Immutable data
    ├── docs       => Documentation of this project
    ├── notebooks  => Notebooks (e.g., Jupyter, R Markdown)
    ├── results    => Tables, figures, etc.
    └── src        => Source code


<!-- END OF README -->
EOF

echo "Top-level README.md file created."
```

# Exercise
## Initialize the repo.

```text
git init .
git add .
git commit -m "Initialize new project repository"
```

# Exercise
## Tell the script to exit cleanly

```text
# All done!
exit 0
```

Your script should return the exit code `0` when it completes without errors.

# Exercise
## Save and quit

Save your file by pressing <kbd>Control</kbd><kbd>o</kbd>.<br/>
Then exit Nano by pressing <kbd>Control</kbd><kbd>x</kbd>.

# Exercise
## Test your script

```
$ ls
make-project.sh
$ bash ./make-project.sh /lustre/isaac/scratch/projects/foo
$ ls -R /lustre/isaac/scratch/projects/foo
```

# Exercise
## Install your script for easy use

```
$ ls
make-project.sh
$ pwd
/lustre/isaac/scratch/USERNAME/src/make-project
$ cd
$ mkdir bin
$ cd bin
$ ln -s /lustre/isaac/scratch/USERNAME/src/make-project/make-project.sh .
$ ls -l
lrwxrwxrwx 1 USERNAME GROUP 63 Feb 29 09:53 make-project.sh -> /lustre/isaac/scratch/USERNAME/src/make-project/make-project.sh
```

# Exercise
## Install your script for easy use

```
$ cd
$ nano .bashrc
```

Add the following text at the end of the file:

```text
alias mkprj="bash ~/bin/make-project.sh"
```

Then exit nano with <kbd>Control</kbd><kbd>o</kbd>, <kbd>Control</kbd><kbd>x</kbd>


<!-- END -->
