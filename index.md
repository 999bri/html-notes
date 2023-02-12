# HTML
https://html.com/
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

## Ordered Lists
Ordered lists (`<ol>`) are like unordered lists, except each list item is numbered. They are useful when you need to list different steps in a process or rank items for first to last. Use `<ol>` then `<li>` toadd individual items. 

Note: Lists can contain videos, images, songs, hyperlinks, or a combination of any - even lists of lists.

## Images
The `<img>` tag allows you to add an image to a web page; this tag is a self-closing tag, but ends with a `/>`. Self-closing tags may include or omit the final slash, but both will render properly. 

The tag has a required attribute called `src`. This attribute must be set to the image's source, or the location of the image; the value of `src` must be the uniform resoure locator (URL) - which is the web address or local address where a file is stored - of the image.

Note: A local address refers to the path to an image, file, or resource located on your own computer. This works with a properly arranged directory or folder structure.

i.e.: `<img src="___" />`

## Image Alts
In order to make a site more inclusive, assistive technologies need to be considered. The `alt` attribute, which means alternative text, brings meaning to the images. It can be added to the image tag just like the `src` attribute. The value of `alt` should be a description of the image.

This attribute also serves the following purposes:
- If an image fails to load, a user can mouse over the area originally intended for the image and read a brief description of the image. 
- Visually impaired users often browse the web with the aid of screen reading software. When you include the `alt` attribute, the screen reading software can read the image's description out loud to the visually impaired user.
- The `alt` attribute also plays a role in Search Engine Optimization (SEO) because search engines cannot "see" the images on the websites. Havin descriptive `alt` attributes can improve the ranking of your site. 

Note: If the image on the web page is not one that conveys any meaningful information to a user (visually impaired or otherwise), the `alt` attribute should be left empty.

i.e.: `<img src="#" alt="A set of tall mountains" />`

## Videos
The `<video>` element requires a `src` attribute with a link to the video source and also requires an opening and a closing tag

i.e.: `<video src="https://content.codecademy.com/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" width="320" height="240" controls>`
          Video not supported
      `</video>`

https://www.codecademy.com/learn/learn-html/modules/learn-html-elements/cheatsheet

https://www.youtube.com/watch?v=uxmB8MlO3m8

## Preparing for HTML
Let your browser know you are using HTML by doing a document declaration; it MUST be your first line of code 
*HTML code is ALWAYS saved in a file with .html extension
i.e.: `<!DOCTYPE html>`

## The HTML Tag
To create HTML content and structure, opening and closing `<html>` tags must be added after declaring document type. Anything in between the opening and closing `<html>` tags will be interpreted as HTML code

## The Head
Give the browser some information about the page itself using the `<head>` element; this contains the metadata for a webpage> Metadata is information about the page that isn't displayed directly on the webpage 

## Page Titles 
opening and closing `<title>` tag is always inside the `<head>` element; the title displays itself on the tab above the URL bar

## Linking to Other Web Pages 
You can add links to a web page by adding an anchor element `<a>`and including the text of the link in between the opening and closing tags; this element depends on the `href` attribute, which stands for hyperlink reference and is used to link to a path or the address to where a file is located 

i.e.: `<a href="https://en.wikipedia.org/wiki/Brown_bear">Learn More</a>`

## Opening Links in a New Window
This could be done using a `target` attribute; this specifies how a link should open. The attribute requires a value of `_blank`. It can be added directly to the opening `<a>` tag just like the `href` attribute.

## Linking to Relative Page
Many sites link to internal web pages like Home, About, Contact. When making sites like this, web developers often store HTML files in the root directory, or a main folder where all the files of the project are stored.

i.e.: project-folder/
      |—— about.html
      |—— contact.html
      |—— index.html
      
This shows three different files in one folder. Since these are stored in the same files, you can link web pages together using a relative path. A relative path is a filename that shows the path to a local file (a file on the same website, such as ./index.html) vs an absolute path (a full URL which is stored in a different folder). The `./` in `./index.html` tells the browser to look for the file in the current folder.

## Linking At Will
HTML allows you to turn nearly any element into a link by wrapping that element with an anchor element. With this technique, it’s possible to turn images into links by simply wrapping the `<img>` element with an `<a>` element.

i.e.: <a href="https://en.wikipedia.org/wiki/Opuntia" target="_blank"><img src="https://www.Prickly_Pear_Closeup.jpg" alt="A red prickly pear fruit"/></a> 
  
## Linking to Same Page
Be able to click a link and have the page automatically scroll to a specific section. In order to link to a target on the same page, we must give the target an id, like this:


## Whitespace
Programmers use two tools to visualize the relationship between elements: whitespace and indentation.

Both tools take advantage of the fact that the position of elements in a browser is independent of the amount of whitespace or indentation in the index.html file.

## Indentation
The World Wide Web Consortium, or W3C, is responsible for maintaining the style standards of HTML. At the time of writing, the W3C recommends 2 spaces of indentation when writing HTML code.

## Comments
Comments begin with <!-- and end with -->. Any characters in between will be ignored by your browser. Comments can span single or multiple lines.

## HTML Tags
https://developer.mozilla.org/en-US/docs/Web/HTML/Element
https://html.com/
https://developer.mozilla.org/en-US/

## Mozilla Development Network [MDN]
It's an open-source network of documentation and tools that has information and a wide variety of topics related to web development, including HTML, CSS, and JavaScript.

MDN articles usually divide content into separate sections. The types of sections will vary depending on the topic, but you will find the following sections in HTML documentation:

A definition and demo - At the top of an MDN article, you’ll see a written definition of the article’s subject. Below the definition, you will find a demo, an interactive example. Here the demo displays a variety of heading elements showing the correct syntax. These demos allow you to run the example code given to you and see the immediate result. You can also interact with the example code including making changes to it.
Attributes - This section describes any attributes specific to the HTML element. In this case, there are none except for global attributes like class or id that are used on all HTML elements.
Usage notes - The section titled “Usage notes” gives helpful tips, including best practices that will help your website follow certain standards.
Examples - This section provides you with even more examples. 
Accessibility concerns - The accessibility concerns section goes over any issues that might impact accessibility, or how easily people can use your website when implementing the code or web technology shown in the article.
Specifications - The specifications section provides links to resources that discuss the article’s topic in more detail. This article’s section goes into the design of these HTML elements, what their purpose is, and how they should function.
Browser compatibility - This section displays information about which web browsers can support, or properly display the HTML elements, discussed in the article. The information found here is similar to the information you would find on a website like caniuse.com although less detailed.
Related topics - There are two sections of this article that will show you additional, related topics: the section “See also” and the sidebar under “Related Topics.” Both provide linked articles that discuss topics related to the subject of the current article.

Except for the Related Topics sidebar, you can jump to the relevant section you want to look at by clicking on the link in the menu, “On this Page,” located at the top of the page.

## Create a Table
Before displaying data, we must first create the table that will contain the data by using the `<table>` element. The `<table>` element will contain all of the tabular data we plan on displaying.
  
## Table Rows
The first step in entering data into the table is to add rows using the table row element: `<tr>`.

## Table Data
Rows aren’t sufficient to add data to a table. Each cell element must also be defined. In HTML, you can add data using the table data element: `<td>`.
`<td>` adds columns with data.

## Table Headings
To add titles to rows and columns, you can use the table heading element: `<th>`. The table heading element is used just like a table data element, except with a relevant title. Just like table data, a table heading must be placed within a table row.
The use of the scope attribute, which can take one of two values:

row - this value makes it clear that the heading is for a row.
col - this value makes it clear that the heading is for a column.

## Table Borders
In older versions of HTML, a border could be added to a table using the border attribute and setting it equal to an integer. This integer would represent the thickness of the border. It's only meant to illustrate older conventions you may come across, otherwise, it's not used. Rather, CSS is used to style and create borders. 
  
## Spanning Columns
Data can span columns using the colspan attribute. The attribute accepts an integer (greater than or equal to 1) to denote the number of columns it spans across.

## Spanning Rows
Data can also span multiple rows using the rowspan attribute. The rowspan attribute is used for data that spans multiple rows (perhaps an event goes on for multiple hours on a certain day). It accepts an integer (greater than or equal to 1) to denote the number of rows it spans across.

## Table Body
## Table Head
## Table Footer
## Styling with CSS
## Introduction to Semantic HTML
## Header and Nav
## Main and Footer
## Article and Section
## The Aside Element
## Figure and Figcaption
## Audio and Attributes
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio#attributes
## Video and Embed 
## How a Form Works
## Text Input
## Adding a Label
## Password Input
## Number Input
## Range Input
## Checkbox Input
## Radio Button Input
## Dropdown list
## Datalist Input
## Textarea element
## Submit Form
