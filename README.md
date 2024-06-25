# Introduction to CSS

HTML provides the skeletal layout of a website. To design and style a website, we use CSS (Cascading Style Sheets). CSS is optional but essential for converting a plain HTML page into a beautiful and responsive website.

## What is CSS?
- **CSS** stands for Cascading Style Sheets.
- **Purpose:** Adds styles to HTML, making the website visually appealing and responsive.

## Installing VS Code
- **Tool:** Microsoft Visual Studio Code
- **Features:** Powerful, free, and customizable.

## Why Learn CSS?
- **Demand:** Highly sought-after skill in web development.
- **Customization:** Enables you to style your website as desired.

## Your First Line of CSS
1. Create a `.css` file in your directory.
2. Add it to your HTML.
3. Example:
   ```css
   /* Sets the background color of the page to red */
   body {
      background-color: red;
   }
   ```

## HTML Refresher
- **HTML:** Uses tags to structure a page.
- **Resources:** Download HTML notes for a detailed deep dive.

## Chapter 1 – Creating Your First CSS Website

### What is DOM?
- **DOM:** Document Object Model, a tree of objects created by the browser when a page is loaded.

### HTML `id` and `class` Attributes
- **id:** Unique identifier for an element.
- **class:** Groups elements together; an element can belong to multiple classes.

Example:
```html
<div id="first" class="class1 class2 class3">
   ...
</div>
```

### Three Ways to Add CSS to HTML
1. **Internal CSS:** Use the `<style>...</style>` tag in HTML.
   ```html
   <style>
   /* Sets the background color of the page to blue */
   body {
      background-color: blue;
   }
   </style>
   ```
2. **Inline CSS:** Use the `style` attribute in an HTML tag.
   ```html
   <div style="color: red;">
      This text is red.
   </div>
   ```
3. **External CSS:** Link a stylesheet using the `<link>` tag.
   ```html
   <link rel="stylesheet" href="styles.css">
   ```

### CSS Selectors
- **Selector:** Used to select HTML element(s) for styling.
  ```css
  /* Selects the body element and sets text color to red and background color to pink */
  body {
     color: red;
     background: pink;
  }
  ```

### Types of Selectors
- **Element Selector:** Selects elements by tag name.
  ```css
  /* Selects all h2 elements and sets their color to blue */
  h2 {
     color: blue;
  }
  ```
- **id Selector:** Selects elements by id.
  ```css
  /* Selects the element with id="first" and sets text color to red and background to black */
  #first {
     color: red;
     background: black;
  }
  ```
- **Class Selector:** Selects elements by class.
  ```css
  /* Selects all elements with class="class1" and sets the background color to red */
  .class1 {
     background: red;
  }
  ```

### Important Notes
- **Grouping Selectors:**
  ```css
  /* Applies the same style to h1, h2, h3, and div elements, setting their color to blue */
  h1, h2, h3, div {
     color: blue;
  }
  ```
- **Elements + Class Selector:**
  ```css
  /* Selects all p elements with class="class2" and sets their color to green */
  p.class2 {
     color: green;
  }
  ```
- **Universal Selector:**
  ```css
  /* Selects all elements and resets margin and padding to 0 */
  * {
     margin: 0;
     padding: 0;
  }
  ```
- **Inline Styles:** Override external and internal styles.

### Comments in CSS
- **Syntax:** Use comments to leave notes or explanations in your CSS code.
  ```css
  /* This is a comment */
  ```

### Practice Set
1. Create a `div` with class `red` that has a red background and white text.
2. Create an element with id `head` and apply inline, external, and style tag CSS to it.
3. Create a CSS class `one` and use it on multiple elements.
4. Apply multiple CSS classes to a single element.
5. Explore the MDN CSS reference for more properties.

## Chapter 2 – Colors & Backgrounds

### Color Property
- **Usage:** Sets text color.
  ```css
  /* Sets the text color to green */
  .class {
     color: green;
  }
  ```

### Types of Color Values
- **RGB:**
  ```css
  /* Sets color using RGB values */
  color: rgb(163, 70, 44);
  ```
- **HEX:**
  ```css
  /* Sets color using HEX code */
  color: #ff0019;
  ```
- **HSL:**
  ```css
  /* Sets color using HSL values */
  color: hsl(67, 78%, 87%);
  ```

### Background Properties
- **background-color:**
  ```css
  /* Sets the background color to greenyellow */
  .class {
     background-color: greenyellow;
  }
  ```
- **background-image:**
  ```css
  /* Sets a background image */
  .class {
     background-image: url('img.png');
  }
  ```
- **background-repeat:**
  ```css
  /* Prevents background image from repeating */
  .class {
     background-repeat: no-repeat;
  }
  ```
- **background-size:**
  ```css
  /* Makes background image cover the container */
  .class {
     background-size: cover;
  }
  ```
- **background-attachment:**
  ```css
  /* Fixes background image in place */
  .class {
     background-attachment: fixed;
  }
  ```
- **background shorthand:**
  ```css
  /* Sets multiple background properties at once */
  .class {
     background: red url(img.png) no-repeat fixed right top;
  }
  ```

### Practice Set
1. Create a dark blue navigation bar with light-colored items.
2. Change the main container color to dark red.
3. Add a background image to a `div` with specific width and height.
4. Create a vertical box with a fixed background.
5. Use the background shorthand property with some values skipped.

## Chapter 3 – CSS Box Model

### Box Model Overview
- **Elements as Boxes:** Margin, Border, Padding, Content.
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
- **Example:**
  ```css
  /* Sets width to 100px and height to 100px */
  .class {
     width: 100px;
     height: 100px;
  }
  ```

### Setting Margin & Padding
- **Example:**
  ```css
  /* Sets margin and padding for all sides to 100px */
  .class {
     margin: 100px;
     padding: 100px;
  }
  ```
- **Individual Margins/Paddings:**
  ```css
  /* Sets individual margin values: top 10px, bottom 10px, left 20px, right 20px */
  .class {
     margin-top: 10px;
     margin-bottom: 10px;
     margin-left: 20px;
     margin-right: 20px;
  }
  ```

### Setting Borders
- **Example:**
  ```css
  /* Sets border width to 3px, style to solid, and color to blueviolet */
  .class {
     border-width: 3px;
     border-style: solid;
     border-color: blueviolet;
  }
  ```
- **Shorthand:**
  ```css
  /* Shorthand for setting border properties */
  .class {
     border: 3px solid blueviolet;
  }
  ```

### Border Radius
- **Example:**
  ```css
  /* Sets rounded borders with a radius of 7px */
  .class {
     border-radius: 7px;
  }
  ```

### Margin Collapse
- **Explanation:** When margins overlap, the larger margin is used.
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
- **Example:**
  ```css
  /* Includes padding and border in element's width and height */
  .class {
     box-sizing:

 border-box;
  }
  ```

### Practice Set
1. Create a layout with a header, content box, and footer.
2. Add borders and margins.
3. Check for margin collapse.
4. Apply box-sizing property and observe changes.

## Chapter 4 – Font & Display

### Display Property
- **inline:** Takes up only the space needed.
  ```css
  /* Sets display to inline */
  .inline-element {
     display: inline;
  }
  ```
- **block:** Takes up the full width and starts on a new line.
  ```css
  /* Sets display to block */
  .block-element {
     display: block;
  }
  ```
- **inline-block:** Similar to inline but allows setting width and height.
  ```css
  /* Sets display to inline-block */
  .inline-block-element {
     display: inline-block;
  }
  ```

### Visibility vs Display
- **display: none;** Removes the element from the document flow.
  ```css
  /* Removes element from document flow */
  .hidden-element {
     display: none;
  }
  ```
- **visibility: hidden;** Hides the element but keeps its space.
  ```css
  /* Hides element but keeps its space */
  .hidden-element {
     visibility: hidden;
  }
  ```

### Text Alignment
- **Example:**
  ```css
  /* Aligns text to the center */
  .text-center {
     text-align: center;
  }
  ```

### Text Decoration
- **Example:**
  ```css
  /* Underlines the text */
  .underlined-text {
     text-decoration: underline;
  }
  ```

### Text Transform
- **Example:**
  ```css
  /* Converts text to uppercase */
  .uppercase-text {
     text-transform: uppercase;
  }
  ```

### Line Height
- **Example:**
  ```css
  /* Sets line height to 1.5 */
  .line-height {
     line-height: 1.5;
  }
  ```

### Font Properties
- **font-family:**
  ```css
  /* Sets font family to Arial */
  .class {
     font-family: Arial, sans-serif;
  }
  ```
- **font-size:**
  ```css
  /* Sets font size to 16px */
  .class {
     font-size: 16px;
  }
  ```
- **font-style:**
  ```css
  /* Sets font style to italic */
  .class {
     font-style: italic;
  }
  ```
- **font-weight:**
  ```css
  /* Sets font weight to bold */
  .class {
     font-weight: bold;
  }
  ```
- **font-variant:**
  ```css
  /* Sets font variant to small-caps */
  .class {
     font-variant: small-caps;
  }
  ```

### Web Safe Fonts
- **Usage:** Universally installed fonts across browsers.
  ```css
  /* Sets font family to Arial */
  .class {
     font-family: Arial, sans-serif;
  }
  ```

### Adding Google Fonts

1. **Go to Google Fonts**: Visit [Google Fonts](https://fonts.google.com/).

2. **Select a Style**: Choose the font and styles you want, for example, "Roboto".

3. **Copy the Link**: After selecting the styles, Google Fonts provides a link.

4. **Include the Link in HTML**: Add this link within the `<head>` section of your HTML file.

5. **Apply the Font in CSS**: Use the selected font in your CSS file to style elements.

Example:

### HTML
Include the link tag within the `<head>` section:
```html
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

### CSS
Apply the font to your elements:
```css
/* Applies Google font 'Roboto' */
body {
   font-family: 'Roboto', sans-serif;
}
```

## Chapter 5 – Size, Position & Lists

### Units for Size
- **Common Units:** `px`, `em`, `rem`, `%`, etc.

This structured approach provides a clear and organized way to understand and apply CSS concepts, keeping it simple and to the point.
