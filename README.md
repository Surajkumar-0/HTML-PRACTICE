# HTML-PRACTICE
HTML practice files and learning journey.

# HTML Journey 🚀

## What is HTML?

HTML (HyperText Markup Language) is the standard markup language used to create and structure web pages. It provides the basic structure of a website using tags and elements.

### Inventor of HTML

* Invented by Tim Berners-Lee
* Introduced in 1991
* Used to create the structure of web pages

---

# 01. Basic HTML Structure

Every HTML document follows a basic structure.

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Page</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```

### Main Elements

#### `<!DOCTYPE html>`

Declares that the document is HTML5.

#### `<html>`

Root element of an HTML page.

#### `<head>`

Contains metadata and page information.

#### `<title>`

Displays the page title in the browser tab.

#### `<body>`

Contains all visible webpage content.

---

# 02. Headings, Paragraphs and Links

## Headings

HTML provides six heading levels.

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

### Notes

* `<h1>` is the most important heading.
* `<h6>` is the smallest heading.
* Headings improve readability and SEO.

## Paragraph

```html
<p>This is a paragraph.</p>
```

Used to display text content.

## Links

```html
<a href="https://google.com">Visit Google</a>
```

### href Attribute

Specifies the destination URL.

---

# 03. Images

Images are added using the `<img>` tag.

```html
<img src="image.jpg" alt="Image">
```

### Important Attributes

#### src

Specifies image location.

#### alt

Alternative text shown if image cannot load.

#### width

Sets image width.

#### height

Sets image height.

Example:

```html
<img src="photo.jpg"
     alt="Photo"
     width="300">
```

### Notes

* `<img>` is an empty tag.
* Images can be local or online.

---

# 04. Tables

Tables are used to display data in rows and columns.

## Basic Tags

### `<table>`

Creates a table.

### `<tr>`

Creates a row.

### `<th>`

Creates a heading cell.

### `<td>`

Creates a data cell.

Example:

```html
<table border="1">
    <tr>
        <th>Name</th>
        <th>Branch</th>
    </tr>

    <tr>
        <td>Suraj</td>
        <td>CSE</td>
    </tr>
</table>
```

## Table Sections

### `<caption>`

Table title.

### `<thead>`

Header section.

### `<tbody>`

Main table content.

### `<tfoot>`

Footer section.

## colspan

Merges columns.

```html
<td colspan="2">Sam</td>
```

## rowspan

Merges rows.

```html
<td rowspan="2">Java</td>
```

---

# 05. Lists

Lists are used to organize items.

## Ordered List

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
</ol>
```

Displays numbered items.

## Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
</ul>
```

Displays bullet points.

## Description List

```html
<dl>
    <dt>HTML</dt>
    <dd>Markup Language</dd>
</dl>
```

### List Tags

* `<ol>` Ordered List
* `<ul>` Unordered List
* `<li>` List Item
* `<dl>` Description List
* `<dt>` Description Term
* `<dd>` Description Description

---

# 06. SEO and Core Web Vitals

## SEO

SEO (Search Engine Optimization) is the process of improving a website's visibility in search engine results.

### Important SEO Tags

#### Title Tag

```html
<title>Learn HTML</title>
```

#### Meta Description

```html
<meta name="description"
content="Learn HTML from beginner to advanced">
```

#### Viewport

```html
<meta name="viewport"
content="width=device-width, initial-scale=1.0">
```

### Semantic HTML

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

Helps search engines understand page structure.

---

# Core Web Vitals

Google uses Core Web Vitals to measure user experience.

## LCP (Largest Contentful Paint)

Measures loading speed.

Good Score:

```text
Less than 2.5 seconds
```

## INP (Interaction to Next Paint)

Measures responsiveness.

Good Score:

```text
Less than 200 milliseconds
```

## CLS (Cumulative Layout Shift)

Measures visual stability.

Good Score:

```text
Less than 0.1
```

### Improving Core Web Vitals

* Use image width and height.
* Optimize images.
* Use lazy loading.
* Write semantic HTML.

---


# 07. HTML Forms and Input Tags

## Introduction

HTML Forms are used to collect data from users. Forms are commonly used for login pages, registration forms, contact forms, surveys, feedback forms, and online applications.

The `<form>` element acts as a container that holds different form controls such as text fields, radio buttons, checkboxes, dropdown lists, and buttons.

---

# Form Tag

The `<form>` tag is used to create a form.

```html
<form action="" method="post">
</form>
```

## Form Attributes

### action

Specifies the location where form data will be sent after submission.

```html
<form action="submit.php">
```

### method

Specifies how form data will be transmitted.

```html
method="get"
```

or

```html
method="post"
```

---

# Input Element

The `<input>` element is used to accept user input.

```html
<input type="text">
```

Input is an empty element and does not require a closing tag.

---

# Common Input Types

## Text Input

Used to enter text such as names and usernames.

```html
<input type="text">
```

---

## Password Input

Used to enter passwords. Characters are hidden for security.

```html
<input type="password">
```

---

## Email Input

Used to enter email addresses.

```html
<input type="email">
```

The browser validates the email format automatically.

---

## Number Input

Used to enter numeric values.

```html
<input type="number">
```

---

## Date Input

Used to select dates from a calendar.

```html
<input type="date">
```

---

## Radio Button

Used when only one option can be selected from a group.

```html
<input type="radio" name="gender" value="male">
<input type="radio" name="gender" value="female">
```

### Important Note

Radio buttons must have the same `name` attribute to work as a group.

---

## Checkbox

Used when multiple options can be selected.

```html
<input type="checkbox" name="hobby" value="cricket">
```

---

## File Input

Used to upload files.

```html
<input type="file">
```

---

## Submit Button

Used to submit form data.

```html
<input type="submit" value="Submit">
```

---

## Reset Button

Used to clear all form fields.

```html
<input type="reset" value="Reset">
```

---

# Label Element

The `<label>` element provides a description for an input field.

```html
<label for="username">Username</label>
<input type="text" id="username">
```

## Benefits

* Improves accessibility.
* Clicking the label focuses the related input field.
* Makes forms more user-friendly.

---

# Important Input Attributes

## id

Provides a unique identifier for an element.

```html
<input type="text" id="username">
```

---

## name

Defines the name of the data sent to the server.

```html
<input type="text" name="username">
```

Example:

```
username = Suraj
```

---

## value

Specifies the value submitted with the form.

```html
<input type="radio" value="male">
```

---

## placeholder

Displays a hint inside the input field.

```html
<input type="text" placeholder="Enter your name">
```

---

## autofocus

Automatically places the cursor inside the field when the page loads.

```html
<input type="text" autofocus>
```

---

## required

Makes a field mandatory.

```html
<input type="email" required>
```

The form cannot be submitted if the field is empty.

---

# Textarea Element

The `<textarea>` element is used for multi-line text input.

```html
<textarea rows="4" cols="50"></textarea>
```

## Attributes

### rows

Defines the height of the textarea.

```html
rows="4"
```

### cols

Defines the width of the textarea.

```html
cols="50"
```

---

# Select and Option Elements

Used to create a dropdown list.

```html
<select name="fruits">
    <option value="apple">Apple</option>
    <option value="banana">Banana</option>
</select>
```

## select

Creates a dropdown menu.

## option

Defines items inside the dropdown.

---

# Data Submission Example

If a user enters:

```
Username : Suraj
Gender : Male
Comment : Learning HTML
Fruit : Banana
```

The server may receive:

```
username = Suraj
gender = male
comment = Learning HTML
fruits = banana
```

---

# Difference Between id and name

| id                          | name                            |
| --------------------------- | ------------------------------- |
| Must be unique              | Can be reused                   |
| Used by CSS and JavaScript  | Used to send data to the server |
| Connects labels with inputs | Identifies form data            |

---

# Advantages of HTML Forms

* Collect user information.
* Enable user interaction.
* Used in login and registration systems.
* Support data validation.
* Essential for web applications.

---

# Conclusion

HTML Forms are used to collect and submit user data. Important form elements include:

* form
* input
* label
* textarea
* select
* option
* button

Forms are one of the most important features of modern web development.


# 08. Inline and Block Elements in HTML

## Introduction

HTML elements are mainly classified into two categories:

* Block Elements
* Inline Elements

Understanding the difference between block and inline elements is essential for designing web pages and learning CSS.

---

# Block Elements

## Definition

A block element always starts on a new line and occupies the full width available by default.

## Characteristics

* Starts on a new line.
* Takes the full available width.
* Width and height can be modified using CSS.
* Other elements appear below it.

## Common Block Elements

* `<div>`
* `<p>`
* `<h1>` to `<h6>`
* `<form>`
* `<table>`
* `<section>`
* `<article>`
* `<header>`
* `<footer>`
* `<nav>`
* `<main>`
* `<ul>`
* `<ol>`
* `<li>`

## Example

```html
<h1>Welcome</h1>

<p>This is my first paragraph.</p>

<div>This is a div element.</div>
```

---

# Inline Elements

## Definition

An inline element does not start on a new line. It only occupies the width required by its content.

## Characteristics

* Does not start on a new line.
* Takes only the required width.
* Multiple inline elements can appear on the same line.
* Mainly used for formatting text and small content.

## Common Inline Elements

* `<span>`
* `<a>`
* `<img>`
* `<b>`
* `<strong>`
* `<i>`
* `<em>`
* `<u>`
* `<mark>`
* `<small>`
* `<sup>`
* `<sub>`
* `<label>`

## Example

```html
I am learning <b>HTML</b> and <i>CSS</i>.
```

---

# Difference Between Block and Inline Elements

| Block Elements                            | Inline Elements                  |
| ----------------------------------------- | -------------------------------- |
| Start on a new line                       | Do not start on a new line       |
| Occupy the full available width           | Occupy only the required width   |
| Used for large sections of a webpage      | Used for small pieces of content |
| Width and height can be easily controlled | Width depends on content         |
| Examples: `div`, `p`, `h1`                | Examples: `span`, `a`, `b`       |

---

# div Element

The `<div>` element is a block-level container used to group large sections of HTML content. It is widely used for page layout and styling with CSS.

## Example

```html
<div>
    <h2>About Me</h2>
    <p>I am learning HTML.</p>
</div>
```

---

# span Element

The `<span>` element is an inline container used to style or group a small portion of text without creating a new line.

## Example

```html
<p>My favorite language is <span>HTML</span>.</p>
```

---

# Key Points

* Block elements begin on a new line.
* Inline elements remain on the same line.
* `<div>` is the most commonly used block element.
* `<span>` is the most commonly used inline element.
* This concept is important before learning CSS because CSS uses `display: block`, `display: inline`, and `display: inline-block`.

---

# Interview Questions

### 1. What is a block element?

A block element starts on a new line and occupies the full available width by default.

### 2. What is an inline element?

An inline element does not start on a new line and occupies only the width required by its content.

### 3. What is the difference between `<div>` and `<span>`?

* `<div>` is a block-level container.
* `<span>` is an inline-level container.

---

# Summary

* HTML elements are divided into block and inline elements.
* Block elements are used for page structure and layout.
* Inline elements are used for formatting text and small content.
* Understanding block and inline elements is important for building responsive web pages and learning CSS.


# 09. ID and Classes in HTML

## Introduction

In HTML, **id** and **class** attributes are used to identify and group elements. They are mainly used for applying CSS styles and selecting elements with JavaScript.

---

# ID Attribute

## Definition

The **id** attribute provides a **unique identifier** for an HTML element. An id value must be unique within a single HTML document.

## Syntax

```html
<p id="intro">Welcome to HTML</p>
```

## Example

```html
<h1 id="title">HTML Tutorial</h1>

<p id="description">
Learn HTML from beginner to advanced.
</p>
```

## Characteristics

* Must be unique on a webpage.
* Used to identify a specific element.
* Commonly used with CSS and JavaScript.
* One element can have only one id.

---

# Class Attribute

## Definition

The **class** attribute is used to group multiple HTML elements under the same name. Multiple elements can share the same class.

## Syntax

```html
<p class="text">Paragraph One</p>
<p class="text">Paragraph Two</p>
```

## Example

```html
<h2 class="heading">HTML</h2>

<p class="heading">
Learning HTML is fun.
</p>
```

## Characteristics

* A class can be used by multiple elements.
* Mainly used for applying the same CSS style to different elements.
* JavaScript can also access elements using class names.
* An element can have multiple classes.

Example:

```html
<div class="box container"></div>
```

---

# Difference Between ID and Class

| ID                            | Class                                           |
| ----------------------------- | ----------------------------------------------- |
| Must be unique                | Can be reused                                   |
| Used for one specific element | Used for multiple elements                      |
| One id per element            | Multiple classes can be assigned to one element |
| CSS Selector: `#id`           | CSS Selector: `.class`                          |

---

# CSS Example

```html
<h1 id="title">Welcome</h1>

<p class="text">HTML Basics</p>

<p class="text">CSS Basics</p>
```

```css
#title{
    color: blue;
}

.text{
    color: green;
}
```

---

# JavaScript Example

Accessing an element by **id**:

```javascript
document.getElementById("title");
```

Accessing elements by **class**:

```javascript
document.getElementsByClassName("text");
```

---

# Best Practices

* Use **id** when you need to identify one unique element.
* Use **class** when multiple elements share the same style or behavior.
* Give meaningful names such as `header`, `navbar`, `btn`, `container`, or `card`.
* Avoid using spaces in id names.
* Follow consistent naming conventions.

---

# Key Points

* `id` identifies a single unique element.
* `class` groups multiple elements together.
* Both attributes are widely used in CSS and JavaScript.
* An element can have only one id but multiple classes.

---

# Interview Questions

### 1. What is the purpose of the id attribute?

The **id** attribute uniquely identifies an HTML element on a webpage.

### 2. What is the purpose of the class attribute?

The **class** attribute groups multiple elements so they can share the same CSS styles or JavaScript behavior.

### 3. Can two elements have the same id?

No. An id must be unique within an HTML document.

### 4. Can multiple elements have the same class?

Yes. Multiple elements can share the same class name.

### 5. Can an element have multiple classes?

Yes.

Example:

```html
<div class="container shadow rounded"></div>
```

---

# Summary

* **id** is used to uniquely identify a single HTML element.
* **class** is used to group multiple elements.
* CSS uses `#` to select an id and `.` to select a class.
* JavaScript can access elements using both id and class.
* Understanding id and class is essential for learning CSS and JavaScript.


# 10. Video, Audio and Media in HTML

## Introduction

HTML5 provides built-in support for multimedia content such as audio and video. Before HTML5, developers had to rely on external plugins like Flash Player to play media files. Today, HTML offers native media elements that work directly in modern web browsers.

The main multimedia elements are:

* `<audio>`
* `<video>`
* `<source>`

---

# Audio Element

## Definition

The `<audio>` element is used to embed and play audio files on a webpage.

## Syntax

```html
<audio src="song.mp3" controls></audio>
```

## Example

```html
<audio src="song.mp3" controls></audio>
```

## Common Audio Attributes

### src

Specifies the location of the audio file.

```html
<audio src="song.mp3"></audio>
```

### controls

Displays the browser's default audio controls such as Play, Pause, Volume, and Progress Bar.

```html
<audio src="song.mp3" controls></audio>
```

### autoplay

Automatically starts playing the audio when the webpage loads.

```html
<audio src="song.mp3" autoplay controls></audio>
```

> Note: Most modern browsers restrict autoplay unless certain conditions are met.

### loop

Repeats the audio continuously.

```html
<audio src="song.mp3" controls loop></audio>
```

### muted

Starts the audio with the sound muted.

```html
<audio src="song.mp3" controls muted></audio>
```

---

# Video Element

## Definition

The `<video>` element is used to embed and play video files on a webpage.

## Syntax

```html
<video src="video.mp4" controls></video>
```

## Example

```html
<video src="video.mp4" controls width="600"></video>
```

---

# Common Video Attributes

### src

Specifies the location of the video file.

### controls

Displays video controls such as Play, Pause, Volume, and Full Screen.

### width

Sets the width of the video.

```html
<video src="video.mp4" width="600" controls></video>
```

### height

Sets the height of the video.

```html
<video src="video.mp4" height="400" controls></video>
```

### poster

Displays an image before the video starts playing.

```html
<video
    src="video.mp4"
    poster="thumbnail.jpg"
    controls>
</video>
```

### autoplay

Starts the video automatically.

### loop

Repeats the video after it finishes.

### muted

Starts the video without sound.

---

# Source Element

## Definition

The `<source>` element is used inside the `<audio>` or `<video>` element to provide multiple media files in different formats.

This helps browsers choose a supported media format.

## Video Example

```html
<video controls width="600">
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    Your browser does not support the video tag.
</video>
```

## Audio Example

```html
<audio controls>
    <source src="song.mp3" type="audio/mpeg">
    <source src="song.ogg" type="audio/ogg">
    Your browser does not support the audio element.
</audio>
```

---

# Supported Media Formats

## Audio Formats

* MP3
* OGG
* WAV

## Video Formats

* MP4
* WebM
* OGG

---

# Advantages of HTML5 Media

* No external plugins are required.
* Supported by all modern browsers.
* Easy to embed audio and video.
* Built-in media controls.
* Better performance and user experience.

---

# Important Attributes Summary

| Attribute  | Description                                   |
| ---------- | --------------------------------------------- |
| `src`      | Specifies the media file location             |
| `controls` | Displays built-in media controls              |
| `autoplay` | Starts media automatically                    |
| `loop`     | Repeats the media continuously                |
| `muted`    | Starts media without sound                    |
| `width`    | Sets video width                              |
| `height`   | Sets video height                             |
| `poster`   | Displays a thumbnail before playing the video |

---

# Interview Questions

### 1. Which HTML tag is used to play audio?

**Answer:** `<audio>`

### 2. Which HTML tag is used to play video?

**Answer:** `<video>`

### 3. What is the purpose of the `controls` attribute?

It displays the default browser controls for playing, pausing, adjusting volume, and navigating media.

### 4. What is the purpose of the `poster` attribute?

It displays a thumbnail image before the video starts playing.

### 5. Why is the `<source>` tag used?

The `<source>` tag allows multiple media formats to be provided so that the browser can choose a supported file.

---

# Key Points

* HTML5 supports multimedia using the `<audio>` and `<video>` elements.
* The `controls` attribute is commonly used to display media controls.
* The `poster` attribute is used only with videos.
* The `<source>` element improves browser compatibility.
* HTML5 media elements eliminate the need for external plugins.

---

# Summary

HTML5 provides built-in support for multimedia content through the `<audio>`, `<video>`, and `<source>` elements. These elements make it easy to embed and play audio and video files while providing features such as playback controls, looping, autoplay, muted playback, and multiple file format support.


# 11. Semantic Tags in HTML

## Introduction

Semantic HTML uses elements that clearly describe the purpose and meaning of the content they contain. Unlike non-semantic elements such as `<div>` and `<span>`, semantic elements make the structure of a webpage easier to understand for developers, browsers, search engines, and assistive technologies.

HTML5 introduced several semantic elements to improve code readability, accessibility, and SEO.

---

# What are Semantic Tags?

Semantic tags are HTML elements that clearly define the meaning and purpose of their content.

## Example

```html
<header>
    <h1>My Website</h1>
</header>
```

The `<header>` element clearly indicates that it represents the header section of a webpage.

---

# Common Semantic Elements

## `<header>`

Represents the introductory section of a webpage or a section. It usually contains the website logo, title, navigation links, or search bar.

### Example

```html
<header>
    <h1>My Portfolio</h1>
</header>
```

---

## `<nav>`

Defines a navigation section that contains links to different pages or sections of a website.

### Example

```html
<nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
</nav>
```

---

## `<main>`

Represents the main content of a webpage. There should generally be only one `<main>` element on a page.

### Example

```html
<main>
    <h2>Welcome to My Website</h2>
</main>
```

---

## `<section>`

Represents a thematic section of related content.

### Example

```html
<section>
    <h2>About Us</h2>
    <p>We provide web development courses.</p>
</section>
```

---

## `<article>`

Represents self-contained content that can be independently distributed or reused, such as blog posts, news articles, or forum posts.

### Example

```html
<article>
    <h2>Introduction to HTML</h2>
    <p>HTML is the standard markup language for web pages.</p>
</article>
```

---

## `<aside>`

Represents content that is indirectly related to the main content, such as sidebars, advertisements, recent posts, or additional links.

### Example

```html
<aside>
    <h3>Recent Posts</h3>
</aside>
```

---

## `<footer>`

Represents the footer section of a webpage or a section. It commonly contains copyright information, contact details, social media links, or legal information.

### Example

```html
<footer>
    <p>&copy; 2026 Suraj Kumar</p>
</footer>
```

---

# Semantic Page Structure

```html
<header>
</header>

<nav>
</nav>

<main>

    <section>
    </section>

    <article>
    </article>

    <aside>
    </aside>

</main>

<footer>
</footer>
```

---

# Advantages of Semantic HTML

* Improves code readability.
* Enhances Search Engine Optimization (SEO).
* Improves website accessibility for screen readers.
* Makes code easier to maintain.
* Helps browsers understand the structure of a webpage.
* Provides meaningful page organization.

---

# Semantic vs Non-Semantic Elements

| Semantic Elements                          | Non-Semantic Elements          |
| ------------------------------------------ | ------------------------------ |
| Have meaningful names                      | Do not describe content        |
| Improve SEO                                | Do not improve SEO directly    |
| Improve accessibility                      | Limited accessibility benefits |
| Easy to understand                         | Generic containers             |
| Examples: `<header>`, `<main>`, `<footer>` | Examples: `<div>`, `<span>`    |

---

# Best Practices

* Use semantic elements whenever possible.
* Use `<header>` for introductory content.
* Use `<nav>` for navigation links.
* Keep only one `<main>` element per webpage.
* Use `<article>` for independent content.
* Use `<section>` to group related content.
* Use `<aside>` for side content.
* Use `<footer>` for footer information.

---

# Interview Questions

### 1. What are semantic tags?

Semantic tags are HTML elements that clearly describe the meaning and purpose of their content.

### 2. Why are semantic tags important?

They improve SEO, accessibility, code readability, and webpage structure.

### 3. Give examples of semantic HTML elements.

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<aside>`
* `<footer>`

### 4. What is the difference between `<div>` and `<section>`?

* `<div>` is a non-semantic container used for grouping elements.
* `<section>` is a semantic element used to group related content with a meaningful purpose.

---

# Key Points

* Semantic HTML provides meaningful structure to web pages.
* HTML5 introduced several semantic elements.
* Semantic elements improve SEO and accessibility.
* They make the code cleaner and easier to maintain.
* Semantic HTML is considered a best practice in modern web development.

---

# Summary

Semantic HTML elements describe the purpose of different sections of a webpage. They help developers write cleaner code, improve accessibility, and allow search engines to better understand webpage content. Using semantic elements is a recommended practice for building modern, well-structured websites.



🚀 This repository documents my HTML learning journey and practice.
