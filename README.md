# Introduction To HTML

![html image](https://cdn.lynda.com/course/170427/170427-637363828865101045-16x9.jpg)

## Overview

We'll be going over the basic's of HTML. In this lesson we'll review everything from creating to a HTML file, to building out a full html page.
This lesson covers HTML syntax and element types.

## Objectives

- Learn how to create an HTML file
- Learn about how an HTML file is structured
- Learn about different HTML tags
- Build a simple HTML page

## What You'll Be Building

![final](Capture.png)

## Getting Started

- Fork and Clone this repository

## What is HTML?

HTML stands for hyper text markup language. It has been in use since the advent of the internet. Every website you visit or interact with is built on or with HTML.

## Creating A HTML File

Inside of this lesson folder, create an `index.html` file. You can either do this in your terminal with `touch index.html` or with vscode's add file button located in your file explorer.

Open the `index.html` file you created. Once the file opens, type `!` and you should see a pop up to use `emmet abbreviations`. Hit the enter key to accept the suggestion. You should be given the following HTML:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

**If emmet did not work for you, feel free to copy and paste the above code into your `index.html`.**

### Stop and Discuss 5 min

Talking points:

- Analyzing the current code
- Why is the file called `index.html`

## HTML Elements

HTML is built with elements or `tags`. For example, the `body` tag is an element. HTML supports many different tags, all of which serve different purposes and uses.

### Block Elements

Block elements, are `tags` that create a box. These elements stack `vertically` on the page in a column format.

Examples of basic block elements:

| Tag    | Uses                                                                       |
| ------ | -------------------------------------------------------------------------- |
| `div`  | A general use containing element                                           |
| `h<n>` | A header tag used to create different sized headings                       |
| `p`    | A paragraph tag to automatically size text to standard paragraph text size |

#### Semantic Tags

Semantic tags, are elements that have a special meaning. These tags aid screen readers in verbally giving feedback for users with disabilities.
Semantic tags were intoduced in the HTML 5 web standard.

Examples of semantic tags:

| Tag       | Uses                                                                                  |
| --------- | ------------------------------------------------------------------------------------- |
| `nav`     | An element that wraps elements for navigation purposes                                |
| `header`  | This element declares a primary heading section or call to action                     |
| `section` | Containing element to break areas of a page into individual sections                  |
| `article` | Containing element to declare articles on a web page                                  |
| `aside`   | A containing element that is typically used to keep elements to the side on webpages. |

### Inline Elements

These elements are used `inline` of block elements. This means that they stack horizontally and do not break up the flow of a page or element.
They are typically used to join groups of HTML elements on a single line.

Examples of inline elements:

| Tag     | Uses                                                                         |
| ------- | ---------------------------------------------------------------------------- |
| `a`     | Anchor tag used for creating links to external sites or different html pages |
| `span`  | `Spans` mutliple elements into a single line                                 |
| `br`    | Breaks text or elements to a new line on the page                            |
| `input` | An element that accepts a user input                                         |
| `img`   | Used for displaying images on a page                                         |

For a full list of HTML elements visit [W3 Schools](https://www.w3schools.com/html/html_blocks.asp)

### Adding Content To Our Page

Head over to your `index.html`. Let's start by adding a nav to our document. Inside of the `nav` tags, add in a `ul` tag followed by 2 `li` tags inside of the `ul`.
The first `li` should contain the text `Home` and the second should contain the text `About`:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
        <nav>
          <ul>
            <li>Home</li>
            <li>About</li>
          </ul>
        </nav>
  </body>
</html>
```

Let's preview our changes. To open the `index.html` file:

- Mac Users: In your terminal use `open index.html`.
- WSL/Windows Users: Right click the `index.html` in your file explorer and select open in explorer. Once the explorer window opens, double click the `index.html`.

**NOTE**: Whenever you make a change to the `index.html`, you must refresh the browser page displaying the file.

Let's add in a `header` and a `section` tag next. The header should come after the closing `nav` tag and before the opening `section` tag.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <nav>
      <ul>
        <li>Home</li>
        <li>About</li>
      </ul>
    </nav>
    <header></header>
    <section></section>
  </body>
</html>
```

### You Do 10 min

Add some content to your page! Here are the necessary requirements, but feel free to add your own flair:

- Must have at least 1 `h1` tag.
- Must have at least 1 `p` tag.
- Must have at least 1 `section` tag.
- The `section` must have 2 `div` tags inside of it.

Feel free to add images if you finish early!

## Element Attributes

All elements within a HTML document have attributes or properties. These properties allow us to differentiate between elements or asign the same style to multiple elements. (More On This Later)

Here's a list of common html attributes:

| Attribute | Use Case                                                                    |
| --------- | --------------------------------------------------------------------------- |
| `id`      | Used to assign unique id to elements                                        |
| `class`   | Used to give elements the same `name` or `class` to style elements the same |
| `href`    | Used with anchor/`a` tags to define a link for navigation                   |
| `src`     | Used with `img` tags to define a source url for an image                    |

For a full list of HTML attributes visit [W3 Schools](https://www.w3schools.com/html/html_attributes.asp)

### Adding Attributes To Our HTML

In your `index.html`, give both of the `li` tags a class of `link`:

```html
<li class="link">Home</li>
<li class="link">About</li>
```

We'll use this class attribute later on to style these elements.

Now give your `section` an `id` attribute of `section-1`:

```html
<section id="section-1">
  <div></div>
  <div></div>
</section>
```

## Recap

In this lesson we learned how to set up a HTML file utilizing semantic tags and attributes.
There's more to HTML than meets the eye! Feel free to use this lesson to experiment with the html file and try different element combinations.

## Resources

- [W3 Schools](https://www.w3schools.com/html/default.asp)
- [35+ HTML/CSS Resources](https://medium.com/level-up-web/30-html-css-resources-for-beginners-4e4d0af4b44b)
