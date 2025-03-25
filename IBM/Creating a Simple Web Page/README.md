# Creating a Simple Web page

## Task_1: Create a new HTML document
in the terminal 
```bash
touch mywebpage.html
```

## Task_2: Specify `<!DOCTYPE>`

This line tells the web browser that the file contains HTML code. This is not an HTML tag.

```html
<!DOCTYPE html>
```

## Task_3: Add the `<head>` and `<body>` elements

An HTML file begins with the `<html> `tag and ends with the corresponding closing `</html>` tag. All HTML code will be placed within these two tags.

The HTML document is divided up into two sections: a *head* and a *body*

The `<head>` tag defines the metadata about the page, which is used by browsers and search engines.
This information may include the document title, character set, styles to be used, scripts, etc.
Contents of `<head>` section are not displayed to the user.

The `<body>` tag defines the document body, and contains all the visible content such as headings, paragraphs, images, links, tables, etc.

```html
<html>
<head>
    <!-- metadata -->
</head>
<body>
    <!-- document body -->
</body>
</html>
```
generate boilerplate code
```html
html:5
```
## Task_4: Add a heading to the page

To add a heading, we will use the `<h1>` tag. This stands for "heading 1" and is used to indicate the most important heading. HTML headings go from `<h1>` to `<h6>`, to represent a descending order of importance.

```html
<h1>Thomas J. Watson</h1>
```
## Task_5: Add a Paragraph

The tag `<p> `is used to define a paragraph.

```html
<p>Thomas J. Watson, Sr. is the American industrialist, who built the International Business Machines Corporation (IBM) into the largest manufacturer of electric typewriters and data-processing equipment in the world.
</p>
```

## Task_6: Add an Image

- An `<img>` tag is used to add an image.
- To add an image you need to know the image file name and mention it in the 'src' attribute.
- The 'src' attribute specifies an external resource that you want to link, such as the URL of an image.
- You can optionally specify how many pixels the width and height of the image should be.

```html
<img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/Thomas_J_Watson_Sr.jpg" width="300" height="300">
```
## Task_7: Create a list

- To create a list of items, we can use the `<ol>` (ordered list) tag for numbered lists, and the `<ul>` (unordered list) tag for bulleted lists.
- Each point within a list will be enclosed by a `<li>` opening and closing tag, which represents a list item. This same tag is used for both ordered and unordered list.

```html
<ul>
    <li>In 1939, he received an honorary degree in Doctor of Commercial Science from Oglethorpe University. </li>
    <li>In 1940s, Watson was on the national executive board of the Boy Scouts of America. </li>
    <li>Watson served as a trustee of Columbia University from June 6, 1933, until his death. </li>
    <li>He was posthumously inducted into the Junior Achievement U.S. Business Hall of Fame in 1990.</li>
</ul>
```

## Task_8: Add a table

- A table is created using the `<table>` tag.
- Within the table, each row of data is represented using the `<tr>` (table row) tag.
- The column or row headings can be specified by the `<th>` (table heading) element.
- Finally, each data element within the table cells is specified using the `<td>` (table data) tag.

```html
table>
    <tr>
        <th>Year </th>
        <th>No. of Employees </th>
        <th>Gross Income (In m$) </th>
    </tr>
    <tr>
        <td>1925</td>
        <td>3698</td>
        <td>13</td>
    </tr>
    <tr>
        <td>1930</td>
        <td>6346</td>
        <td>19 </td>
    </tr>
    <tr>
        <td>1935</td>
        <td>8651</td>
        <td>21</td>
    </tr>
    
</table>
```

## Task_9: Add Links to other pages

- Web pages connect to other web pages and files using hyperlinks.
- A hyperlink is created using the anchor tag `<a>`
- Once you click the link, the `href `attribute tells the browser which web page you should be taken to.

```html
 <a href="https://www.ibm.com">IBM</a>
```

## Task_10: Add a Feedback Form

Let's create a feedback form to collect user input. Forms are an essential part of web development, allowing for the collection and submission of data to a server. They provide an interactive way for users to enter text, make selections, and submit information for processing.
To build this form, we will use the following HTML elements:

- `<form>`:
Defines the structure of the form and acts as a container for all form-related elements. It specifies where and how the collected data should be submitted.

- `<input>`:
Collects user input through various types such as text, email, password, and more, allowing for single-line data entry.

- `<textarea>`:
Allows users to input larger amounts of text, such as comments or feedback, providing a scrollable, multi-line input area.

- `<button>`:
Used to trigger specific actions, such as submitting or resetting the form. The behavior is determined by the type attribute.

- `<label>`:
Provides a textual description or context for form controls, improving usability and accessibility, especially for screen readers.

- `<fieldset>`:
Groups related elements in a form, visually and logically organizing them. Often used with a `<legend>` to describe the group.

```html
<h2>Insights Submission Form</h2>
    <form action="/submit-feedback" method="POST">
        <fieldset>
            <legend>Your Insights About Thomas J. Watson Are Valued</legend>
    
            <!-- Name Field -->
            <label for="name">Name:</label><br>
            <input type="text" id="name" name="name" placeholder="Enter your name" required><br><br>
    
            <!-- Email Field -->
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" placeholder="Enter your email" required><br><br>
    
            <!-- Comments Field -->
            <label for="comments">Comments:</label><br>
            <textarea id="comments" name="comments" rows="4" cols="50" placeholder="Share your thoughts about Thomas J. Watson"></textarea><br><br>
    
            <!-- Submit Button -->
            <button type="submit">Submit</button>
        </fieldset>
    </form>
```
