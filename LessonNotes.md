# Intro
- What is HTML?
  - Hypertext markup language
  - A set of pre-defined tags that tell a browser how to display text
    - Blank text file + HTML tags = website!
- Tags
  - Instruction how to display content on a screen
  - ex: `<h1> Hello World </h1>`
  - The Sandwich Model of HTML tags
    - tags are like bread, content is like meat
  - Make sure closing tags have forward slash!
- Attributes
  - Additional value that configures or adjusts behaviour of a tags
  - ex: `<button class="btn"> Press Me </button>`
  - Attributes are import for linking to CSS styles (id, class)
  - Tags can be removed or not written in the first place

# Layout
- Block level vs Inline
  - block level elements take up whole width of their container
  - inline elements take up only a much space as they need
-`<span>``
  - generic inline container
  - used to keep text together inline
- `<p>`
  - paragraph of text
  - block level elements
  - used when wanting to write a paragraph
- ``<div>``
  - generic block container
  - good way to divide up website
  - can be styled with CSS

## Demo

# Typesetting
- superscript ``<sup>``
- subscript ``<sub>``
- underline ``<u>``
- italics ``<em>``
- bold ``<strong>``
- break line ``<br>`` *Does not need a closing tag*
- horizontal rule ``<hr>`` *does not need a closing tag*

# Container tags
- Our website needs a few special tags to contain all the other tags
- ``<!DOCTYPE>``
  - tells the browser what kind of file it is reading
  - simply `<!DOCTYPE html>`
- ``<html>``
  - root element of an html document
  - right after doctype
  - only used once in a given pages
- ``<head>``
  - provides general info and important links for setting up the page
  - Not displayed
  - ``<title>`` to be displayed in browser tab
  - ``<charset>`` defines which set of ASCII characters to use
    - mostly utf-8
  - For the most part, CSS and JS will be imported here:
    - `<link rel="stylesheet" href="./style.css" />`
- ``<body>``
  - content actually displayed on pages


# Lists
- ``<ol>``
  - ordered list
  - ex.
    1. abo
    2. pebo
    3. max rebo
- ``<ul>``
  - unordered list
  - ex.
    - just a man
    - living life
    - on the prairie
- ``<li>``
  - list item
  - actual content of lists
  - nested part of an HTML list

# Headers
- `<h1> - <h6>`
  - adds heading above a certain element
  - block level item
  - h1 > h2 > h3 ... > h6

# Links
- ``<a>``
  - Anchor tag, creates a hyperlink
  - tons of attributes, most important is `href`, hyperlink reference
  - content of tag will link to url in `href` attributes
  - can link to external sites with http (absolute path)
    - ex: `<a href="http://www.reddit.com"> Stay away from this site </a>`
  - link to internal pages with relative path
    - ex: `<a href="recipe.html"> a delicious kimchi recipe</a>`
# Images
- `<img>`
  - Inserts images
  - inline element
  - closing tag is most commonly placed in opening tag
  - src attribute defines path to image to be displayed (required)
  - alt attribute describes photo if photo can't be displayed
  - ex: `<img src="images/kimchi.jpg" alt='a batch of fully fermented kimchi'/>`
  - style attribute can be helpful to tweak size of image

# CSS
- Cascading Style Sheets
  - Cascading describes the system used by the browser to determine which rules to apply to a particular piece of content -- it 'cascades' from more general to more specific rules, choosing the most specific
- Goes inside of a style tag that goes inside head tag
  - ex: `<link rel="stylesheet" href="./style.css" />`
- Links HTML elements with style instructions
- Written in a new document in same folder as html files (often `styles.css`)
- CSS syntax
  - name of element followed by styling instructions
  - dot `.`  before name if using class attribute
  - hash `#` if referring to id attribute
  - no prefix if referring to standard html tag
  - styling instructions contained in curly brackets `{}`
  - style type followed by colon `:`
  - value follows colon
  - each style ends in semicolon `:`
    - ex, a paragraph with 30pt blue text with sans-serif font and a gray background:
    ```CSS
    .intro {
      color: blue;
      font-size: 30pt;
      font-family: sans-serif;
      background-color: gray;
    }
    ```

# Custom Fonts
- Find a font you like at `fonts.google.com`
- Selecting it
- Copy standard code into head of webpage `.html file`
- Reference font in CSS rules to use
