# HTML and CSS Milestones

**Note**: This is still just a skeleton, will be filled out later, based on material I've compiled over the years.

## Contents <!-- omit in toc -->

- [Instructions](#Instructions)
- [Demonstrations: Helpful and Unhelpful](#Demonstrations-Helpful-and-Unhelpful)
  - [Helpful Demonstrations](#Helpful-Demonstrations)
  - [Unhelpful Demonstrations](#Unhelpful-Demonstrations)
- [Milestones](#Milestones)
- [Development Environment](#Development-Environment)
  - [Command Line](#Command-Line)
  - [Editing and Viewing](#Editing-and-Viewing)
  - [Publishing HTML](#Publishing-HTML)
- [HTML Fundamentals](#HTML-Fundamentals)
  - [Basic Structure](#Basic-Structure)
  - [The Anatomy of an HTML Tag](#The-Anatomy-of-an-HTML-Tag)
  - [Basic Tags](#Basic-Tags)
  - [Lists](#Lists)
  - [Tables](#Tables)
  - [Multimedia](#Multimedia)
- [CSS](#CSS)
  - [Identifying CSS](#Identifying-CSS)
  - [Styling A Page](#Styling-A-Page)
  - [Semantic HTML and Logical Structure](#Semantic-HTML-and-Logical-Structure)
  - [Common Page Features and Layouts](#Common-Page-Features-and-Layouts)
  - [Responsive Design](#Responsive-Design)
  - [JavaScript in the Browser](#JavaScript-in-the-Browser)

## Instructions

## Demonstrations: Helpful and Unhelpful

### Helpful Demonstrations

### Unhelpful Demonstrations

## Milestones

## Development Environment

### Command Line

You should be able to...

- [ ] Open the terminal outside of VS Code
- [ ] Use `cd` to navigate between directories
- [ ] Use `ls` to list the contents of a directory
- [ ] Use `mkdir` to create an empty directory
- [ ] Use `touch` to create an empty file
- [ ] Use `code` to open VS Code

### Editing and Viewing

- [ ] Create a new (empty) project directory
- [ ] In the new project directory, create a new (empty) HTML file named `index.html` and edit it in VS Code
- [ ] Write some HTML in `index.html`
- [ ] Open `index.html` in your browser and view it locally
- [ ] Add an image to the project directory and display it on the webpage using the `<img>` tag

### Publishing HTML

- [ ] Use [surge.sh][url-surge-sh] to publish the project to the web
- [ ] Validate your HTML using [validator.w3.org][url-w3-validator]
- [ ] Create a [CNAME][url-surge-sh-remember-domain] file each project so that surge doesn't generate a new, random domain every time you publish

## HTML Fundamentals


### Basic Structure

Let's make sure we have the basic structure of an HTML page down. Don't worry too much about the content, here.

You should be able to create a file called `structure.html` that contains the following, structured correctly:

- [ ] A `DOCTYPE` declaration
- [ ] A `<html>` tag, containing...
  - [ ] A `<head>` tag, containing...
    - [ ] A `<title>` tag with a title of your choosing
  - [ ] A `<body>` tag containing...
    - [ ] One top-level `<h1>` header
    - [ ] A few paragraphs of text in `<p>` tags
    - [ ] A second-level `<h2>` tag
    - [ ] A few more paragraphs of text in `<p>` tags

### The Anatomy of an HTML Tag

You should be able to create a properly structured HTML document named `snippet.html` that talks about the following snippet:

```html
<p>
  Want to search the web?
  Try <a href="https://google.com" id="the-best-link" class="banana"  target="_blank">Google</a>!
</p>
```

In `snippet.html`, you should be able to:

- [ ] Name the tags in the snippet
- [ ] Link to 2-3 online references that describe each tag, give examples, etc.
- [ ] Describe the relationship between the tags in terms of nesting ("X is a child of Y")
- [ ] Explain the relationship between `<p>` and `</p>`
- [ ] Explain the relationship between `<a>` and `</a>`
- [ ] List the attribute names on the `<a>` tag
- [ ] For each attribute on the `<a>` tag, name its value
- [ ] For each attribute/value pair on the `<a>` tag, describe its purpose and effect

### Basic Tags

Using a single-column layout, create a page called `basic-tags.html` that contains the following sections. There should be a single `<h1>` tag for the entire page and a single `<h2>` tag for each section.

Each section should be contained in its own `<section>` tag. Do not use any CSS to style the appearance of the page. Focus just on the HTML. We will create a styled copy later that we can compare side-by-side with the unstyled copy.

You should be able to create sections that demonstrate...

- [ ] The following block-level text containers:
  - [ ] The paragraph `<p>` tag
  - [ ] The blockquote `<blockquote>` tag
  - [ ] The pre-formatted text `<pre>` tag
- [ ] Inline text styling using the following tags:
  - [ ] `<em>` and `<i>`
  - [ ] `<strong>` and `<b>`
  - [ ] `<code>`
- [ ] The `<a>` tag
- [ ] The `<img>` tag
- [ ] The different header tags `<h1>`, `<h2>`, `<h3>`, etc.

### Lists

Building on `basic-tags.html`, you should be able to do the following:

- [ ] Create multiple unordered lists using the `<ul>` and `<li>` tags
- [ ] Create multuple ordered lists using the `<ol>` and `<li>` tags
- [ ] Include other HTML inside the list item (`<li>`) tags, e.g., paragraphs, images, links, etc.
- [ ] Nest lists within each other

### Tables

Building on `basic-tags.html`, you should be able to create tables of varying sizes:

- [ ] Create a 3x3 table using the `<table>`, `<tr>`, and `<td>` tags
- [ ] Add headings using the `<th>` tag
- [ ] Create two more tables of different dimensions

### Multimedia

Create a page named `multimedia.html` in which you:

- [ ] Use the `<video>` tag to embed one or more videos
- [ ] Use the `<audio>` tag to embed one or more audio clips

## CSS

### Identifying CSS

You should be able to create a page called `selectors.html` that demonstrates the following by using a `<style>` tag to include the CSS:

- [ ] Selectors...
  - [ ] Type / tag selectors
  - [ ] Class selectors
  - [ ] ID selectors
- [ ] Combinators...
  - [ ] Descendant combinator
  - [ ] Child combinator

### Styling A Page

You should be able to create a copy of `basic-tags.html` called `basic-tags-styles.html` and do the following:

1. Give each section its own distinct `id`
1. Use a class selector to change the color of some (but not all) of the text on the page. You will need to add `class` attributes to various elements.
1. Change the text color of the `<h2>` header in the first section using an id selector, tag selector, and child combinator
1. Add borders to some (but not all) of the sections. Consider giving the sections you want to have borders the same `class` attribute and then using a class selector.

### Semantic HTML and Logical Structure

The browser has no opinion about the *meaning* of your HTML document. Why is the HTML document organized one way versus another? What do your choice of tags and class/ID names represent? Are there conventions you're following?

To the browser, an HTML document consists of a bunch of nested elements. Some of those elements have a default style, but virtually every aspect can be changed via CSS. Using CSS, you can make every `<p>` tag look and act like an `<h1>` tag, if you want.

These *semantics* are important for the author and any other people who want to make sense of the HTML document down the road, including the author's future self.

### Common Page Features and Layouts

- [ ] Header
- [ ] Footer
- [ ] 2-Column Layout
- [ ] 3-Column Layout
- [ ] Grid

### Responsive Design

### JavaScript in the Browser

- [ ] Listening to events
- [ ] DOM Nodes
  - [ ] **C**reate
  - [ ] **R**ead
  - [ ] **U**pdate
  - [ ] **D**estroy

[url-surge-sh]: http://surge.sh/
[url-surge-sh-remember-domain]: http://surge.sh/help/remembering-a-domain
[url-w3-validator]: https://validator.w3.org/
