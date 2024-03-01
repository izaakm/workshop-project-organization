---
title: Documentation
---

# Documentation

<!-- blank slide -->

# Documentation

Your README file ...

- is a form of documentation that provides a general overview of the package.
- is the first thing other developers will look at.
- should be a plain text file.
- may be writting with Markdown formatting (README.md).

~ <https://en.wikipedia.org/wiki/README>

# README.md
## Markdown

```
$ cat README.md
```

```text
# Example Project

This is the description of my example project.

## Setup/Installation

1. Clone this repo:
    ```
    $ git clone https://github.com/GITHUB_USERNAME/example-project.git
    ```
2. Then `cd` and `pip install`:
    ```
    $ cd example-project
    $ pip install .
    ```
```

# What *is* Markdown?

Simple, text-based formatting instructions (**markup**).

# Why use Markdown?

<table>
<tr>
<td>
![](images/readme-terminal/main.png)
</td>
<td>
![](images/readme-github/main.png)
</td>
</tr>
</table>

# Why use Markdown?

![](images/readme-terminal/main.png)


# Why use Markdown?

![](images/readme-github/main.png)


# Why use Markdown?

- Easy to read in **plain-text** (e.g., in the terminal).
- Nice to read online ... and more.
    <div class="footnote"> these slides are written in Markdown </div>

# Headings

Markdown:

```text
# A first-level heading or title
## A second-level heading
```

What it looks like:

<!-- example headings --> 

## A first-level heading or title

### A second-level heading

<!-- end of slide --> 

# Headings
## ... on GitHub


GitHub automatically generates a table of contents at the top of the file, and
you can click a title to navigate to the selected section.

![](https://docs.github.com/assets/cb-82878/mw-1440/images/help/repository/headings-toc.webp)

[headings]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings


# Formatting
## Text

| Markdown               | What it looks like online |
| -                      | -                         |
| `*This is italicized*` | *This is italicized*      |
| `**This is bold**`     | **This is bold**          |
| `` `This is code` ``   | `This is code`            |


# Formatting
## Code blocks

Markdown: 

````text
```
echo "Hello World"
```
````

What it looks like:

```
echo "Hello World"
```


# Formatting
## Code blocks w/ syntax highlighting

Markdown: 

````text
```bash
echo "Hello World"
```
````

What it looks like:

```bash
echo "Hello World"
```

# Links

Markdown:

```text
A link to [Google.com](https://www.google.com).
```

What it looks like:

A link to [Google.com](https://www.google.com).


# Lists

Markdown:

```text
- George Washington
* John Adams
+ Thomas Jefferson
```

What it looks like:

- George Washington
* John Adams
+ Thomas Jefferson


# Numbered lists

Markdown:

```text
1. James Madison
2. James Monroe
3. John Quincy Adams
```

What it looks like:

1. James Madison
2. James Monroe
3. John Quincy Adams


# Exercise

1. Add Markdown formatting to your README




<!-- END -->
