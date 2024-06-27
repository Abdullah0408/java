# Introduction to HTML

## What is HTML?
HTML (HyperText Markup Language) is the standard language for creating websites. It structures a webpage and its content using a series of elements to define different parts of a webpage.

## Why HTML, CSS, and JavaScript?
- **HTML**: Defines the structure and layout of a webpage.
- **CSS**: Adds styling to the HTML structure.
- **JavaScript**: Adds interactivity and logic to the webpage.

### Analogy:
- **HTML**: The car body (only metal).
- **CSS**: The car paint and decorations.
- **JavaScript**: The car engine and interior logic.

## Setting Up Your Environment
To begin working with HTML, you can use any text editor. Here's how to set up using VS Code:

1. **Installing VS Code**: Download this lightweight, open-source text editor from Microsoft. Search "VS Code" on Google to find and download it.

### Note:
HTML can be written in any text editor, including Notepad.

# Chapter 1 – Creating Our First Website

## Basic HTML Page Structure
To start building a website, create a file named `index.html`. This file is special because it is presented when the website's root address is typed. Here's a basic structure of an HTML page:

```html
<!DOCTYPE html>  <!-- Specifies this is an HTML 5 document -->
<html> <!-- Root element of the HTML page -->
<head> <!-- Contains metadata about the document -->
   <title>Document</title> <!-- Title of the document -->
</head> <!-- Closing head tag -->
<body> <!-- Main body of the page (rendered by the browser) -->
  <h1>Hello</h1> <!-- Heading tag -->
  <p>This is HTML</p> <!-- Paragraph tag -->
</body> <!-- Closing body tag -->
</html> <!-- HTML page ends here -->

## HTML Elements
An HTML element consists of a start tag, content, and an end tag. For example:

```html
<p>This is a paragraph.</p>
```

- Start tag: `<p>`
- Content: This is a paragraph.
- End tag: `</p>`

### Important Notes
- **Children and Parent Tags**: `<head>` and `<body>` are children of `<html>`. `<html>` is the parent of `<head>` and `<body>`.
- **Element Structure**: Most HTML elements have opening and closing tags with content in between. Some tags, like `<br>`, are empty.
- **Extensions**: You can use `.htm` or `.html` extensions.
- **Viewing HTML**: Use “Inspect Element” or “View Page Source” in Chrome to view a website’s HTML code.

## Comments in HTML
Comments in HTML are used to mark text which should not be parsed. They can help document the source code.

```html
<!-- This is a comment -->
```

### Case Sensitivity
HTML is case insensitive. `<H1>` and `<h1>` are the same.

## Practice
- **Inspect Element**: Inspect your favorite website and change something on the page.
- **View Source**: View the page source of your favorite website and write the exact lines of code. Does it clone the website? Why or why not?
- **Write HTML**: Write HTML code inside a text file using Notepad. Does it work if you open the file in a web browser?

By understanding these basics and how to put them together, you can start creating beautiful websites easily!

# Chapter 2 – Basic HTML Tags

In this chapter, we will cover the basic HTML tags that define the structure and content of a webpage. Understanding these tags is essential for creating well-structured and semantically correct HTML documents.

## HTML Elements and Attributes

### HTML Element
An HTML element is composed of a start tag, content, and an end tag.

```html
<tagname>Content</tagname>
```

### HTML Attributes
Attributes provide additional information about HTML elements. They are always included in the opening tag and come in name/value pairs like `name="value"`.

```html
<a href="https://google.com">Click here</a>
```

## Basic Tags

### Heading Tags
Headings are used to define the headings of a page. HTML provides six levels of headings, `<h1>` to `<h6>`, with `<h1>` being the most important.

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
```

### Paragraph Tag
The `<p>` tag is used to define paragraphs in HTML.

```html
<p>This is a paragraph.</p>
```

### Anchor Tag
The `<a>` tag defines hyperlinks, which are used to link from one page to another.

```html
<a href="https://google.com">Click here</a>
```

### Image Tag
The `<img>` tag is used to embed images in an HTML page. It is an empty element, meaning it has no closing tag.

```html
<img src="image.jpg" alt="Description of the image">
```

### Bold, Italic, and Underline Tags
These tags are used to emphasize text.

```html
<b>This is bold text</b>
<i>This is italic text</i>
<u>This is underlined text</u>
```

### Line Break Tag
The `<br>` tag is used to create a line break within text.

```html
<p>This is a line of text.<br>This is another line of text.</p>
```

### Horizontal Rule Tag
The `<hr>` tag is used to create a horizontal line, which can be used to separate content.

```html
<hr>
```

### Subscript and Superscript Tags
These tags are used to display text as subscript or superscript.

```html
<sub>This is subscript</sub>
<sup>This is superscript</sup>
```

### Preformatted Text Tag
The `<pre>` tag is used to display preformatted text. The text inside this tag is displayed in a fixed-width font, and whitespace is preserved.

```html
<pre>
  This is preformatted text.
  It preserves spaces and line breaks.
</pre>
```

## Useful HTML Character Entities

HTML character entities are used to display reserved characters or to express characters that are not available on the keyboard.

| Result | Description               | Name  | Number |
|--------|---------------------------|-------|--------|
|        | non-breaking space        | &nbsp;| &#160; |
| <      | less than                 | &lt;  | &#60;  |
| >      | greater than              | &gt;  | &#62;  |
| &      | ampersand                 | &amp; | &#38;  |
| "      | double quotation mark     | &quot;| &#34;  |
| '      | single quotation mark     | &apos;| &#39;  |
| ¢      | cent                      | &cent;| &#162; |
| £      | pound                     | &pound;| &#163; |
| ¥      | yen                       | &yen; | &#165; |
| €      | euro                      | &euro;| &#8364; |
| ©      | copyright                 | &copy;| &#169; |
| ®      | trademark                 | &reg; | &#174; |

## Block and Inline Elements

### Block Elements
Block elements create a block-level box and always start on a new line in the document. Examples include:


`<address>`
`<article>`
`<aside>`
`<blockquote>`
`<canvas>`
`<dd>`
`<div>`
`<dl>`
`<dt>`
`<fieldset>`
`<figcaption>`
`<figure>`
`<footer>`
`<form>`
`<h1>-<h6>`
`<header>`
`<hr>`
`<li>`
`<main>`
`<nav>`
`<noscript>`
`<ol>`
`<p>`
`<pre>`
`<section>`
`<table>`
`<tfoot>`
`<ul>`
`<video>`


### Inline Elements
Inline elements create an inline-level box and do not start on a new line in the document. Examples include:


`<a>`
`<abbr>`
`<acronym>`
`<b>`
`<bdo`
`<big>`
`<br>`
`<button>`
`<cite>`
`<code>`
`<dfn>`
`<em>`
`<i>`
`<img>`
`<input>`
`<kbd>`
`<label>`
`<map>`
`<object>`
`<output>`
`<q>`
`<samp>`
`<script>`
`<select>`
`<small>`
`<span>`
`<strong>`
`<sub>`
`<sup>`
`<textarea>`
`<time>`
`<tt>`
`<var>`


## Practice Set

1. **Create a Basic HTML Page**: Create a webpage with a title, a main heading, and a subheading.
   - Tags to use: `<html>`, `<head>`, `<title>`, `<body>`, `<h1>`, `<h2>`
   
2. **Add an Image**: Create a page with five wallpaper images taken from the internet.
   - Tags to use: `<img>`
   
3. **Use Line Breaks and Horizontal Rules**: Display a piece of text with line breaks and a horizontal rule.
   - Tags to use: `<p>`, `<br>`, `<hr>`
   
4. **Write a Chemical Equation**: Write the chemical equation for the reaction of carbon and oxygen to form carbon dioxide using subscript and superscript tags.
   - Tags to use: `<sub>`, `<sup>`
   
5. **Clone a Webpage**: Try to clone a simple webpage by viewing its source code and replicating the structure in your own HTML file.

By practicing these examples, you will gain a solid understanding of basic HTML tags and their usage in creating simple web pages.

Certainly! Here's the continuation of the reformatted content:

# Chapter 3 – Creating a Page Layout

When we use the right tags in the right place, it results in a better page layout, improved indexing by search engines, and a better user experience.

## Semantic HTML Tags

### Header, Main, and Footer Tags

These tags help define the structure of your webpage.

```html
<header>
  <!-- Website header content -->
</header>
<main>
  <!-- Main content of the website -->
</main>
<footer>
  <!-- Website footer content -->
</footer>
```

### Section, Aside, and Article Tags

Inside the `<main>` tag, we use the following tags to structure the content:

```html
<main>
  <section>
    <!-- A section of the page -->
  </section>
  <aside>
    <!-- Self-contained content, like a sidebar -->
  </aside>
  <article>
    <!-- Independent, self-contained content -->
  </article>
</main>
```

Using these tags creates a readable and structured layout, which is also useful for SEO.

## Link Attributes

### Creating Links

Use the anchor (`<a>`) tag to create links.

```html
<a href="/contact.html">Contact Us</a> <!-- Opens in the same tab -->
<a href="/contact.html" target="_blank">Contact Us</a> <!-- Opens in a new tab -->
```

You can put any content inside an anchor tag (images, headings, etc.).

### Linking to Images

You can add links to images like this:

```html
<a href="/about.html">
  <img src="image.jpg" width="120" alt="About Us">
  <!-- Height will be set automatically -->
</a>
```

## Div and Span Tags

### Div Tag

The `<div>` tag is often used as a container for other elements. It is a block-level element, meaning it takes up the full width available.

```html
<div>
  <!-- Content here -->
</div>
```

### Span Tag

The `<span>` tag is an inline container, meaning it only takes up as much width as necessary.

```html
<span>
  <!-- Content here -->
</span>
```

## Practice

1. **Create an SEO-friendly website**: Use semantic HTML tags to create a well-structured page.
2. **Link an image to a page**: Create an HTML page that opens Google when an image is clicked.
3. **Bookmark your top websites**: Create a webpage with links to your top five most-used websites, with each link opening in a new tab.

By using these tags and attributes correctly, you can create a well-structured, SEO-friendly, and user-friendly website.

# Chapter 4 – Lists, Tables, and Forms

## Lists

### Unordered List
Used to list unordered items.

```html
<ul>
  <li>Home</li>
  <li>Projects</li>
</ul>
```

### Ordered List
Used to list ordered items.

```html
<ol>
  <li>Phone</li>
  <li>PC</li>
  <li>Laptop</li>
</ol>
```

## Tables

### Basic Table Structure

```html
<table>
  <caption>Table Caption</caption>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
  </tbody>
</table>
```
- **`<table>`**: Defines a table.
- **`<caption>`**: Optional element for providing a caption to the table.
- **`<thead>`**: The header section of the table, typically containing column headers (`<th>` elements).
- **`<th>`**: Defines a header cell within the `<thead>`, typically used for column headings.
- **`<tbody>`**: The body section of the table, containing the main content (`<tr>` elements).
- **`<tr>`**: Defines a row in the table.
- **`<td>`**: Defines a standard data cell within a `<tr>`, used for displaying data.

### Colspan and Rowspan

```html
<table border="1">
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
  <tr>
    <td colspan="2">Cell 3 (spans 2 columns)</td>
  </tr>
  <tr>
    <td rowspan="2">Cell 4 (spans 2 rows)</td>
    <td>Cell 5</td>
  </tr>
  <tr>
    <td>Cell 6</td>
  </tr>
</table>
```

### Diagram:
```
+-------------------+-------------------+
|      Cell 1       |      Cell 2       |
+-------------------+-------------------+
|   Cell 3 (2 cols)                     |
+-------------------+-------------------+
| Cell 4 (2 rows)   |      Cell 5       |
+                   +-------------------+
|                   |      Cell 6       |
+-------------------+-------------------+
```
- **`colspan="2"`**: Indicates that the cell spans across 2 columns horizontally.
- **`rowspan="2"`**: Indicates that the cell spans across 2 rows vertically.

## Forms

### Basic Form Structure

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <input type="submit" value="Submit">
</form>
```

### Form Elements

- Text Input: `<input type="text">`
- Checkbox: `<input type="checkbox">`
- Radio Button: `<input type="radio">`
- Button: `<input type="button">`
- Submit: `<input type="submit">`
- Textarea: `<textarea></textarea>`
- Dropdown: `<select><option>Option 1</option></select>`

## Embedding Video

### Video Tag
Used to embed a video file.

```html
<video src="video.mp4" controls width="400">Video not supported</video>
```

- **Common Attributes**:
  - `controls`: Adds video controls (play, pause, etc.).
  - `autoplay`: Automatically starts the video.
  - `loop`: Loops the video.
  - `width` and `height`: Set the dimensions of the video.

### Embedding YouTube Video

Use an iframe to embed a YouTube video.

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
```

## Practice

1. Create an HTML page with an embedded video.
2. Replace the video with a YouTube video.
3. Create an HTML form for booking a vacation.
4. Create a table displaying cricket players' scores.

# Chapter 5 – SEO

## Types of SEO

- **On-page SEO**: Can be done by HTML developers.
- **Off-page SEO**: Involves activities outside the website to improve search engine rankings.

## HTML SEO Techniques

- Set a concise and relevant title.
- Add a meta description: `<meta name="description" content="...">`
- Use appropriate URL slugs.
- Add meta keywords and author tags: `<meta name="author" content="...">`
- Set a favicon.
- Compress images and other resources.
- Remove unused HTML/CSS/JS and compress them.
- Add alt text to images: `<img src="image.jpg" alt="description">`

This guide provides a foundational understanding of HTML, CSS, and JavaScript, along with practical examples and exercises to reinforce learning.
