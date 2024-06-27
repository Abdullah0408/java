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


