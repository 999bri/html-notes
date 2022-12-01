# HTML
## Intro to HTML
HTML stands for HyperText Markup Language:
- a markup language is a computer language that defines the structure and presentation of raw text
- in HTML, the computer can interpret raw text that is wrapped in HTML elements
- HyperText is text displayed on a computer or device that provides access to other text through links, also known as hyperlinks

## The Body
`<body>` `</body>`

Many different types of content like text, images, and buttons can be added into the body.

## HTML Structure
When an element is contained inside another element, it is considered the child of that element; nested; they are either separated by an indentation or two spaces for better readability 

Since there are multiple levels of nesting, the analogy can be extended to grandchildren, great-grandchildren, etc. This is known as hierarchy.

## Headings
In HTML, there are six different headings or heading elements. These headings are sorted from largest to smallest. `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`

## Divs
`<div>` is short for "division" or a container that divides the page into sections; useful for grouping elements; no visual representation, but useful when wanting to apply custom styles through CSS

They could also contain any text or other HTML elements, such as links, images, or videos. 

## Attributes
Attributes are content added to the opening tag of an element and can be used in several different ways, from providing information to changing styling.

They are made up of the following two parts:
- the name of the attribute
- the value of the attribute

One commonly used attribute is `id`. This attribute is used to specify different content like `<div>`s and helpful when using an element more than once.

i.e.:
`<div id="intro">`

## Displaying Text
If you want to display text, you could use a paragraph or span:
- paragraphs (`<p>`) contain a block of plain text
- `<span>` contains short pieces of text or other HTML; used to separate small pieces of content that are on the same line as other content; best to use when targeting a specific piece of content that is *inline* or on the same line as other text (important later on CSS)

If you want to divide content into blocks, it's better to use `<div>`. 

i.e.:

`<div>`

  `<p>` `<span>`Skulls`</span>` are a bone protective layer for the brain.`</p>`
  
`</div>`

## Styling Text
`<em>` tag emphasizes text; generally renders as italic emphasis 
`<strong>` tag highlights important text; generally renders as bold emphasis

## Line Breaks
Line breaks are used to modify the spacing/positioning in the browser using `<br>`; it can be used anywhere within the code 

## Unordered Lists
In HTML, an unordered list tag (`<ul>`) is used to create a list of items in no particular order. It outlines individual list items with a bullet point.
This element should not hold raw text and won't automatically format raw text into an unordered list of items. 

Individual list items must be added to the unordered list using the `<li>` tag; this is used to describe an item in a list

Note: using raw text will only lead to an error.

i.e.:

`<ul>`

  `<li>` limes `</li>`
  
  `<li>` tortillas `</li>`
  
`</ul>`


