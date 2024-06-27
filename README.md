# Introduction to CSS

HTML provides the basic structure of a website, but CSS is what we use to design and style it, transforming a simple HTML layout into an attractive and responsive web page.

## What is CSS?

CSS stands for Cascading Style Sheets. While it is optional, CSS is essential for converting a plain HTML page into a visually appealing and responsive one.

## Installing VS Code

We'll use Microsoft Visual Studio Code (VS Code) to edit our code. VS Code is a powerful, free, and customizable tool that's ideal for web development.

## Why Learn CSS?

CSS is a highly sought-after skill in web development. Mastering CSS allows you to customize your website to match your vision and design preferences.

## Your First Line of CSS

To start using CSS, create a `.css` file in your project directory and link it to your HTML file. Add the following code to your CSS file to change the background color of your page to red:

```css
/* This will set your page background to red */
body {
    background-color: red;
}
```

## HTML Refresher

HTML consists of various tags that form the structure of a web page. For a detailed deep dive, download the accompanying HTML notes. If you're already familiar with basic HTML, you're ready to move forward!

## Chapter 1 – Creating Our First CSS Website

In this chapter, we'll create our first CSS-styled website.

### What is the DOM?

The Document Object Model (DOM) is a tree structure that represents the contents of a web page. When a page loads, the browser creates a DOM, enabling us to interact with and manipulate the structure using scripts.

### HTML `id` and `class` Attributes

- **`id` Attribute:** Assigning an `id` to an HTML element gives it a unique identifier. Each `id` must be unique within the document.
- **`class` Attribute:** Assigning a `class` to an HTML element allows it to be part of a group. Multiple elements can share the same class, and an element can have multiple classes.

Example:
```html
<div id="first" class="class1 class2 class3">
   ...
</div>
```

### Three Ways to Add CSS to HTML

1. **Using the `<style>` Tag:** Add `<style>...</style>` within the HTML.
2. **Inline CSS:** Use the `style` attribute directly within HTML elements.
3. **External CSS:** Link a separate stylesheet (`.css`) file using the `<link>` tag.

### CSS Selectors

CSS selectors are used to target HTML elements for styling.

- **Basic Structure:**
```css
body { 
   color: red;         /* Sets text color to red */
   background: pink;   /* Sets background color to pink */
}
```

- **Element Selector:** Targets elements by their tag name.
```css
h2 {
   color: blue;       /* Sets text color of all <h2> elements to blue */
}
```

- **ID Selector:** Targets elements by their unique `id`.
```css
#first { 
   color: red;        /* Sets text color to red for the element with id="first" */
   background: black; /* Sets background color to black for the element with id="first" */
}
```

- **Class Selector:** Targets elements by their class name.
```css
.class1 {
   background: red;   /* Sets background color to red for all elements with class="class1" */
}
```

### Important Notes

- **Grouping Selectors:** Apply the same styles to multiple elements.
```css
h1, h2, h3, div {
   color: blue;       /* Sets text color to blue for all <h1>, <h2>, <h3>, and <div> elements */
}
```

- **Combining Elements and Classes:** Target specific elements with a class.
```css
p.class2 {
   color: green;      /* Sets text color to green for all <p> elements with class="class2" */
}
```

- **Universal Selector:** Targets all elements.
```css
* {
   margin: 0;         /* Removes default margin from all elements */
   padding: 0;        /* Removes default padding from all elements */
}
```

- **Inline Styles:** Override both external and internal styles.

### Comments in CSS

Comments are ignored by the browser and used to add notes within the CSS.
```css
/* This is a comment */
```

### Chapter 1 – Practice Set

1. Create a website with a `div` class named `red` that has a red background color and white text.
2. Create an element with the `id` `head` and apply background color styles using inline, external, and internal CSS.
3. Create a CSS class named `one` and apply it to multiple elements to ensure it works correctly.
4. Create multiple CSS classes and apply them to the same element to verify they work together.
5. Refer to the [MDN CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) and experiment with various CSS properties and values.

### Chapter 2 – Colors & Backgrounds

CSS rules consist of simple key-value pairs with selectors. In this chapter, we'll explore how to change colors and set backgrounds using CSS.

### The `color` Property

The CSS `color` property sets the text color inside an element. It can be used to specify colors for various elements.

### Types of Color Values

Here are the most commonly used color values in CSS:

- **RGB:** Specifies color using red, green, and blue values.
  ```css
  color: rgb(163, 70, 44); /* Example */
  ```

- **HEX Code:** Specifies color using hexadecimal code.
  ```css
  color: #ff0019; /* Example */
  ```

- **HSL Code:** Specifies color using hue, saturation, and lightness values.
  ```css
  color: hsl(67, 78%, 87%); /* Example */
  ```
  - **HSL:** `hue`, `saturation`, `lightness`

**Note:** There are also RGBA and HSLA values for color, which include an alpha value representing opacity. These are less commonly used by beginners.
- **RGBA:** `rgb(red, green, blue, alpha)`
- **HSLA:** `hsl(hue, saturation, lightness, alpha)`

### The `background-color` Property

The CSS `background-color` property specifies the background color of an element.

Example:
```css
.class {
   background-color: greenyellow;
}
```

### The `background-image` Property

This property sets an image as the background of an element.

Example:
```css
.class {
   background-image: url('img.png');
}
```
The image repeats by default in both the x and y directions.

### The `background-repeat` Property

Controls the repetition of the background image.

Examples:
- `repeat-x`: Repeats the background image horizontally.
- `repeat-y`: Repeats the background image vertically.
- `no-repeat`: Does not repeat the background image.

For more possible values, refer to the [MDN documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat).

### The `background-size` Property

Defines the size of the background image.

Examples:
- `cover`: Scales the image to cover the element, no empty space.
- `contain`: Scales the image to be fully visible within the element.
- `auto`: Displays the image in its original size.
- `{width or height}`: Sets width, and the height is set automatically (or vice versa).
- `{width, height}`: Sets both width and height.

### The `background-attachment` Property

Specifies whether the background image is fixed or scrolls with the rest of the page.

Example:
```css
.class {
   background-attachment: fixed;
}
```

### The `background` Shorthand Property

Allows setting multiple background properties in one declaration.

Example:
```css
.class {
   background: red url('img.png') no-repeat fixed right top;
   /*        color  image          repeat   attachment  position */
}
```
One or more properties can be omitted as long as the order is maintained.

### Chapter 2 – Practice Set

1. Create a dark blue navigation bar with light-colored items.
2. Change the background color of the main container on your page to dark red.
3. Create a `div` and add a background image with specified width and height.
4. Create a vertical box and add a fixed, non-scrolling background to it.
5. Verify that the `background` shorthand property works with some of the values skipped.

### Chapter 3 – CSS Box Model

The CSS box model treats all HTML elements as boxes.

```
+-------------------------------+
|         Margin Area           |
|  +-------------------------+  |
|  |       Border Area       |  |
|  |  +-------------------+  |  |
|  |  |    Padding Area   |  |  |
|  |  |  +-------------+  |  |  |
|  |  |  |   Content   |  |  |  |
|  |  |  +-------------+  |  |  |
|  |  +-------------------+  |  |
|  +-------------------------+  |
+-------------------------------+
```

### Setting Width & Height

You can set the width and height of an element in CSS as follows:

```css
.class {
   width: 100px;
   height: 100px;
}
```

**Note:** The total width/height is calculated as:
```
total width/height = width/height + left & right/top & bottom padding + left & right/top & bottom border + left & right/top & bottom margin
```

### Setting Margin & Padding

Margins and padding can be set in several ways:

```css
.class {
   margin: 100px;      /* sets top, bottom, left, and right values */
   padding: 100px;
}
```

For individual sides:

```css
.class {
   margin: 1px 2px 3px 4px;  /* top, right, bottom, left */
}
```

or:

```css
.class {
   margin: 2px 4px;  /* top & bottom, left & right */
}
```

You can also set individual margins/paddings:

```css
.class {
   margin-top: 10px;
   margin-bottom: 10px;  /* same goes for padding */
   margin-left: 20px;
   margin-right: 20px;
}
```

### Setting Borders

Borders can be set as follows:

```css
.class {
   border-width: 3px;
   border-style: solid;
   border-color: blueviolet;
}
```

or using shorthand:

```css
.class {
   border: 3px solid blueviolet;  /* shorthand */
}
```

### Border Radius

To create rounded borders:

```css
.class {
   border-radius: 7px;
}
```

### Margin Collapse

When two margins from different elements overlap, the resulting margin is the greater of the two. This is called margin collapse.

Example:
```
+------------------+
|      .box1       |
+------------------+
|                  |  Collapsed Margin (30px)
|                  |  The larger of .box1's bottom margin (30px)
|                  |  and .box2's top margin (20px)
+------------------+
|      .box2       |
+------------------+
```

### Box Sizing

Determines what parts of the box (padding and border) are included in the element's width and height. 

- **content-box:** (default) Includes only content in width/height.
- **border-box:** Includes content, padding, and border in width/height.

```css
.class {
   box-sizing: border-box; /* width and height include content, padding, and border */
}
```

### Chapter 3 – Practice Set

1. Create a website layout with a header box, one content box, and a footer.
2. Add borders and margin to one of the boxes.
3. Check if the margin collapses between the content box and the footer.
4. Add the `box-sizing` property to the content box and note any changes.

### Chapter 4 – Font & Display

In this chapter, we'll explore the `display` property and various font-related properties in CSS to enhance the look and feel of a website.

### The `display` Property

The CSS `display` property determines how an element is displayed on the page, whether as a block, inline element, or other layout types like flexbox or grid.

#### `display: inline`

An inline element takes only the space required by the content, without line breaks before or after it. Width, height, margin, and vertical padding are generally ignored.

```css
.inline-element {
   display: inline;
   background-color: lightblue;
   padding: 10px 20px; /* Only horizontal padding affects layout */
   margin: 10px 20px;  /* Only horizontal margin affects layout */
   width: 100px;       /* Ignored */
   height: 50px;       /* Ignored */
}
```

#### `display: block`

A block element takes the full width available and leaves a newline before and after it.

```css
.block-element {
   display: block;
}
```

#### `display: inline-block`

An inline-block element is similar to an inline element, but allows setting width, height, margin, and padding. Elements can sit next to each other.

```css
.inline-block-element {
   display: inline-block;
   width: 100px;
   height: 50px;
   margin: 10px;
   padding: 10px;
}
```

#### `display: none` vs `visibility: hidden`

- **`display: none`:** The element is removed from the document flow, and its space is not reserved.
- **`visibility: hidden`:** The element is hidden, but its space is still reserved.

### `text-align` Property

The `text-align` property sets the horizontal alignment of text within an element.

```css
.text-center {
   text-align: center;
}
```

### `text-decoration` Property

The `text-decoration` property is used to decorate the text, such as adding an underline, overline, or line-through.

```css
.underline {
   text-decoration: underline;
}
```

### `text-transform` Property

The `text-transform` property specifies the capitalization of text.

```css
.uppercase {
   text-transform: uppercase;
}
```

### `line-height` Property

The `line-height` property sets the space between lines of text.

```css
.spacing {
   line-height: 1.5;
}
```

### Fonts

Fonts play a crucial role in the look and feel of a website.

#### `font-family`

The `font-family` property specifies the font of the text and can hold multiple values as a fallback system.

```css
.font-example {
   font-family: Arial, Helvetica, sans-serif;
}
```

#### Web Safe Fonts

Web safe fonts are universally installed across browsers, ensuring consistency.

#### Adding Google Fonts

To use custom Google Fonts, go to Google Fonts, select a style, and paste the provided link into the `<head>` section of your HTML. Then, use the font in your CSS.

```html
<!-- Example of adding Google Fonts in HTML -->
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

```css
body {
   font-family: 'Roboto', sans-serif;
}
```

#### Other Font Properties

- **`font-size`:** Sets the size of the font.
  ```css
  .large-text {
     font-size: 20px;
  }
  ```

- **`font-style`:** Sets the font style (e.g., italic).
  ```css
  .italic-text {
     font-style: italic;
  }
  ```

- **`font-weight`:** Sets the weight of the font (e.g., bold).
  ```css
  .bold-text {
     font-weight: bold;
  }
  ```

- **`font-variant`:** Sets whether text is displayed in small-caps.
  ```css
  .small-caps {
     font-variant: small-caps;
  }
  ```

### Generic Font Families

Generic families are broad classes of similar fonts, such as serif or sans-serif. The `font-family` property can specify both specific and generic font families.

```css
body {
   font-family: 'Times New Roman', Times, serif; /* Specific and generic families */
}
```

### Chapter 4 – Practice Set

1. Create a navigation bar with inline elements.
2. Create a footer with block elements.
3. Create a text box with a specific font family and a fallback font.
4. Use Google Fonts for custom typography on your website.
5. Experiment with different `display` properties and note the changes in layout.

### Chapter 5 – Size, Position & Lists

In this chapter, we'll discuss different units for sizing, positioning elements, and styling lists in CSS.

### Size Units

There are more units for describing size other than `px`. Some common ones include `rem`, `em`, `vw`, `vh`, and percentages.

#### What's Wrong with Pixels?

Pixels (`px`) are relative to the viewing device. For a device with a resolution of 1920x1080, 1px is 1 unit out of 1920 horizontally and 1080 vertically. This can make designs look inconsistent across different devices.

#### Relative Lengths

These units are relative to other length properties. Here are some commonly used relative lengths:

- **em**: Unit relative to the parent element's font size. `1em` means "my parent element's font size."
- **rem**: Unit relative to the root element's font size (usually the `<html>` tag).
- **vw**: Unit relative to 1% of the viewport's width.
- **vh**: Unit relative to 1% of the viewport's height.
- **%**: Unit relative to the parent element's size.

### Min/Max Height and Width Properties

CSS has `min-height`, `max-height`, `min-width`, and `max-width` properties.

- If the content is smaller than the minimum height, the minimum height will be applied.
- Similarly, if the content is larger than the maximum height, the maximum height will be applied.

### The `position` Property

The `position` property is used to manipulate the location of an element. Here are the possible values:

- **static**: The default position. `top`, `bottom`, `left`, `right`, and `z-index` have no effect.
- **relative**: The element's position is adjusted relative to its normal position. `top`, `bottom`, `left`, and `right` will now work.
- **absolute**: The element is removed from the document flow and positioned relative to its first non-static ancestor.
- **fixed**: The element is positioned relative to the browser window and remains in place even when the page is scrolled.
- **sticky**: The element is positioned based on the user's scroll position.
