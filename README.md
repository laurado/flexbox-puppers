# Flexbox Clinic

## Introduction
This is a simple HTML and CSS project to teach students how to lay out a web page using Flexbox.

## Setup
To get set up, clone this repository and open the `index.html` file in your browser

## Lesson Topics
  * History
  * Introduction
  * Flex Containers and Flex Items
  * Horizontal Alignment
  * Vertical Alignment
  * Wrapping Flex Items
  * Rows vs. Columns

### History
  * In the past, floats and the default box model were used for laying out web pages
  * Floats are somewhat limiting (and are a bit of a hack)

### Introduction
  <!-- CSS Native? -->
  * Flexbox is a relatively new technology, but we're at a point where support is fairly widespread across browsers
  * It gives us control over alignment, direction, order, and size of our boxes
  * Used to define overall page structure

### Flex Containers and Flex Items
  * We manipulate the items we want to style (Flex Items) through the parent (Flex Containers)
  <!-- * Only the direct children  -->


Enable Flexbox layout mode with the following **property** and **value**.

```
.flex-container {
  display: flex;
}
```

<!-- | Property     | Value        |
| ------------ |:------------:|
| display      | flex         | -->

This tells the browser that everything in the container should be rendered with Flexbox instead of the default box model. Otherwise the browser will ignore all Flexbox properties.

### Horizontal Alignment
  * To align Flex Items horizontally, use the `justify-content` property

Possible values include:

| Values       |
| ------------ |
| center       |
| flex-start   |
| flex-end     |
| space-around |
| space-between|

### Vertical Alignment
  * To align Flex Items vertically, use the `align-items` property
  * NOTE: You must define a height for your container to use this property, otherwise the container will only be as tall as the content

Possible values include:

| Values       |
| ------------ |
| center       |
| flex-start (top) |
| flex-end (bottom)    |
| stretch | Useful for equal height columns with a variable amount of content in each
| baseline|

### Wrapping Flex Items
  * The `flex-wrap` property can be used to create a grid
  * This is more powerful than float based grids because you can change alignment, direction, order, and size

Possible values include:

| Values       |
| ------------ |
| wrap       | Forces items that don't fit to get bumped to the next row
| nowrap   |

### Rows vs. Columns
