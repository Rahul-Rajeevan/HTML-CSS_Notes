# Topics to be discussed
1. Meta tags
2. Semantic tags
3. Creating forms
4. Creating tables
5. Linters

# HTML document structure

## Detailed Explanation

Imagine you're building a house. Like any house, there's a basic structure and blueprint you need to follow to ensure it stands firm and functions properly. In the world of the web, HTML (HyperText Markup Language) provides the blueprint for how a website should look and function.

Let's dive into this analogy:

### 1. **Doctype Declaration (`<!DOCTYPE html>`):**

- **Analogy:** Think of the Doctype as the building permit for your house. Before you start building, you need to declare what type of building it is.
- **Importance:** The Doctype tells the web browser which version of HTML the page is written in. This ensures that the browser renders the page correctly according to the rules of that HTML version.

### 2. **HTML (`<html>`):**

- **Analogy:** This is the plot of land where your house will stand. Everything you build will be within this plot.
- **Importance:** The `<html>` tag encapsulates all the content of an HTML document. It tells the browser that everything inside it is HTML content.

### 3. **Language (`lang` attribute):**

- **Analogy:** Think of the `lang` attribute as the region or country where your house is located. Just as different regions might have different building standards or styles, websites can have different languages.
- **Importance:** It's important for accessibility. Screen readers use this attribute to pronounce words correctly. It also helps search engines understand the primary language of the content.

### 4. **Head (`<head>`):**

- **Analogy:** This is like the foundation and utilities of your house: water, electricity, and gas lines. While they aren't visible or flashy, they are essential for the house to function.
- **Importance:** The `<head>` section contains meta information, links to stylesheets, scripts, and other resources that are essential for the proper presentation and behavior of the web page.

### 5. **Meta Tags (`<meta>`):**

- **Analogy:** These are the specifications and labels on your utility lines and foundation. They provide additional information about the house, like its energy efficiency or the capacity of the water heater.
- **Importance:** Meta tags provide essential information to browsers and search engines about the content and character of a page. Common meta tags include charset (character encoding), viewport (for responsive design), and description (which provides a brief overview of the site for search engines).

### 6. **Body (`<body>`):**

- **Analogy:** Now we're talking about the visible part of the house: walls, rooms, windows, and doors. This is where you live, decorate, and interact.
- **Importance:** The `<body>` tag contains everything that a user will see and interact with on the web page. This is where you put your content: text, images, videos, links, and more.

---


# Meta tags

## Introduction

- Meta tags are vital components within the `<head>` section of an HTML document. They provide metadata about the document's content or give instructions to browsers on how to display it. While not directly visible on the page, meta tags can influence how web pages are described and displayed in search results.

## Detailed Explanation

- **What is the concept?** - 
The <meta> tag in HTML is used to provide metadata about the HTML document. Metadata is data about data, and in the context of HTML, it includes information like the character set, page description, keywords, author, and viewport settings.

- **Why is it useful?** -
Here are some of the most common meta tags and their purposes:

1. Charset (`<meta charset="UTF-8">`):
    - **Description:** Specifies the character encoding for the HTML document.
    - **Importance:** It ensures characters in the document are rendered correctly, especially for languages with special characters.
    - Ascii: https://www.w3schools.com/charsets/ref_html_ascii.asp
    - Emojis: https://www.w3schools.com/html/html_emojis.asp
    
2. Viewport (`<meta name="viewport" content="width=device-width, initial-scale=1">`):
    - **Description:** Defines how a page should appear on mobile devices and is crucial for responsive design.
    - **Importance:** It ensures the website scales and sizes properly on all devices, especially mobile ones.
    
3. Description (`<meta name="description" content="A brief summary of the webpage's content">`):
    - **Description:** Provides a short and concise summary of the webpage's content.
    - **Importance:** Search engines often display this description in search results. A good description can entice users to click on your link.
    
4. Keywords (`<meta name="keywords" content="keyword1, keyword2, ...">`):
    - **Description:** Originally used to tell search engines what keywords the page should rank for.
    - **Importance:** Today, this tag holds less weight in search engine ranking algorithms due to over-optimization and keyword stuffing in the past. Some argue its relevance is minimal now.
5. Author (`<meta name="author" content="Name of the author">`):
    - **Description:** Specifies the author of the webpage.
    - **Importance:** Lets readers know who created the content, though it's not widely used for SEO purposes.
6. Refresh (`<meta http-equiv="refresh" content="5;url=https://example.com/">`):
    - **Description:** Automatically refreshes the page or redirects to another after a specified number of seconds.
    - **Importance:** Can be useful in certain situations like after a form submission or for timed redirects, but overuse can degrade user experience.



## Instructor Activity | Code Implementation | Examples
Implement a meta tag that refreshes a page every 5 seconds.

## Student Activities
Implement a meta tag that redirect the user to masaischool.com after 5 seconds.


## Resources - Official Documentation and Other Resources
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta

---


# Semantic Tags

- Semantic HTML elements are those that introduce meaning to web content. Unlike non-semantic elements like `<div>` and `<span>`, which don't convey specific meanings on their own, semantic elements clearly define their content for both the browser and the developer.

Using semantic elements not only makes the code more readable and maintainable but also benefits accessibility tools like screen readers and search engine optimization (SEO) efforts.

## Detailed Explanation

- **What is the concept?** - 
Semantic tags in HTML are elements that describe the meaning of the content they contain, rather than just its presentation. These tags provide context to the content, making it easier for search engines, screen readers, and other tools to understand the structure and purpose of the web page.

1. <header>
Description: Represents a container for introductory content or navigation links. Often contains the website logo, website's title, and main navigation.
Example:
```html
<header>
  <h1>Website Name</h1>
  <nav>
    <!-- navigation links -->
  </nav>
</header>
```
​
2. <nav>
Description: Denotes a section with navigation links, either within the current document or to other documents.
Example:
```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
  </ul>
</nav>
```
​
3. <main>
Description: Represents the main content of a document. There should be only one <main> per page, and it should be unique from content that is repeated across a set of documents such as site navigation, header, or footer.
Example:
```html
<main>
  <article>
    <!-- main content -->
  </article>
</main>
```
​
4. <article>
Description: Represents self-contained content that makes sense on its own and can be independently distributed or syndicated.
Example:
```html
<article>
  <h2>Blog Post Title</h2>
  <p>Blog post content...</p>
</article>
```
​
ChatGPT Chat: https://chat.openai.com/share/e154d280-ce3f-48cb-9710-2689e2512af2 

5. <section>
Description: Represents a standalone section of a document, like tabs of content or a set of content grouped under a theme.
Example:
```html
<section>
  <h2>Section Title</h2>
  <p>Section content...</p>
</section>
```
​
6. <aside>
Description: Used for content that is tangentially related to the main content and can be considered separate. Often seen as sidebars in a design.
Example:
```html
<aside>
  <h3>Related Links</h3>
  <ul>
    <!-- list of links -->
  </ul>
</aside>
```
​
7. <footer>
Description: Represents the footer of a document or a section, typically containing information about the author, copyright information, or related documents.
Example:
```html
<footer>
  <p>Copyright © 2023</p>
</footer>
```

- **Why is it useful?** -
1. **Accessibility:** Semantic elements are crucial for screen readers and other assistive technologies. They convey the structure and role of the content, helping users navigate and understand it better.
2. **SEO:** Search engines reward well-structured content, and semantic elements make it easier for search engines to identify and index the content properly.
3. **Maintainability:** Semantic elements convey meaning, making it easier for developers to understand the structure and purpose of content in a document.
4. **Styling:** CSS frameworks and browser defaults often provide styles tailored to semantic elements, giving you a head start in designing.



## Instructor Activity | Code Implementation | Examples
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semantic tags</title>
    <!---Semantic tags in HTML are elements that convey meaning about the structure and content of a web page to both the browser and the developer.-->
</head>
<body>
    <header> <!--- Represents the header of a section or the entire page. It typically contains site branding, navigation menus, and other introductory content. --->
        <h1>Welcome to My Web Page</h1>
        <nav> <!---Defines a navigation menu, such as a site menu or a table of contents for a page-->
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main> <!---Represents the main content of the document. There should be only one <main> element per page-->
        <section> <!---Represents a thematic grouping of content within a page. It helps to organize content into meaningful sections.-->
            <h2>About Us</h2>
            <p>Welcome to our website! We are a team of passionate individuals dedicated to providing you with valuable information.</p>
        </section>

        <section>
            <h2>Services</h2>
            <ul>
                <li><strong>Web Design:</strong> We create beautiful and functional websites.</li>
                <li><strong>Graphic Design:</strong> Our designs will <mark>make your brand stand out.</mark></li>
                <li><strong>SEO:</strong> We optimize your website for search engines.</li>
            <!---<strong> is used to emphasize text.-->
            <!--  Represents text that has been highlighted or marked for reference, often with a yellow background. -->
            </ul>
        </section>

        <section>
            <h2>Contact Us</h2>
            <address> <!---<address> is used to define contact information.-->
                <p>Email: <a href="mailto:contact@example.com">contact@example.com</a></p>
                <p>Phone: <a href="tel:+123456789">+1 (234) 567-89</a></p>
            </address>
        </section>
    </main>

    <footer> <!---It typically contains copyright information, contact details, and other closing content.-->
        <p>&copy; 2023 My Web Page</p>
    </footer>
</body>
</html>


```



## Resources - Official Documentation and Other Resources
- https://developer.mozilla.org/en-US/docs/Glossary/Semantics


---

# Forms in HTML

- Forms are a fundamental aspect of web development and are used to gather information from users. An HTML form is defined using the <form> element. Inside the form, you can have various types of input elements to collect different kinds of data.

## Detailed Explanation

- **What is the concept?** - 



###  1. `<input>`

The `<input>` element is the most versatile form control. It can be configured in various ways depending on its `type` attribute. Some popular input types include:

- `text`: For single-line text input.
- `password`: Similar to `text` but hides the characters as they're typed.
- `radio`: Lets users select one option among a set.
- `checkbox`: Lets users select zero or more options of a limited number of choices.
- `submit`: A button to submit the form.
- `reset`: A button to reset the form to its initial state.
- `file`: For file uploads.
- `hidden`: A hidden data field, which doesn't show to the user but can store data to be sent with the form.
- `date`, `time`, `datetime-local`: For date and time input.
- `email`: For email input. It can validate if the inputted text is in the format of an email address.
- `url`: For URL input. Validates the input format as a URL.
- `number`: Input for numbers. You can set minimum, maximum, and step values.

### 2. `<textarea>`

Allows multi-line text input.

### 3. `<select>`

Used to create a drop-down list. The options within the list are defined using `<option>` elements.

### 4. `<button>`

A clickable button.

### 5. `<label>`

Provides a textual description for a form control. It helps in improving accessibility. When a user clicks on a label, it gives focus to the form element it is associated with.

- **Why is it useful?** -
Data Collection: Forms allow websites to collect various types of data from users, such as text inputs, selections, checkboxes, radio buttons, and more. This data can be anything from simple contact information to complex survey responses.

Interactivity: Forms enable interactivity on websites by allowing users to input data, make selections, and submit information. This interactivity enhances user engagement and interaction with the website.

User Feedback: Forms can be used to gather feedback from users, whether it's about the website itself, products or services offered, or any other aspect. This feedback is valuable for improving user experience and making informed decisions.

User Authentication: Forms are commonly used for user authentication purposes, such as login and registration forms. They allow users to securely input their credentials to access restricted areas of the website or to create new accounts.

E-commerce: Forms play a crucial role in e-commerce websites by enabling users to input shipping addresses, payment information, and other details necessary for completing purchases.

Search and Filtering: Search forms allow users to input search queries, while filtering forms enable users to refine search results based on various criteria. These forms enhance the usability of websites with large amounts of content.

Data Validation: Forms can include validation rules to ensure that users input data in the correct format and within acceptable ranges. This helps maintain data integrity and improves the overall quality of the collected information.

Accessibility: Properly structured forms with appropriate labels and input elements contribute to the accessibility of websites, making them usable by people with disabilities who rely on assistive technologies.



## Instructor Activity | Code Implementation | Examples
Use MDN and create a form with input, text-area, select, submit, etc.

## Student Activities
Use MDN and create a form with input, text-area, select, submit, etc.


## Resources - Official Documentation and Other Resources
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form


---

# Table in HTML

- An HTML table is used to represent data in a tabular format, i.e., in rows and columns. This structure can be immensely useful for displaying information in a structured manner, like financial statements, calendars, and various kinds of lists.
## Detailed Explanation

- **What is the concept?** - 
Here's a basic breakdown of table-related elements:

### 1. `<table>`

This is the root element for a table. All other table elements are nested within it.

### 2. `<thead>`

This element wraps the set of rows that describe the table headers. Although not strictly required, it's useful for differentiating the header row(s) from the body rows.

### 3. `<tbody>`

This element wraps the set of rows that describe the actual data in the table. It is also not strictly required, but it's a good semantic element to differentiate the main content of the table from the headers and footers.

### 4. `<tfoot>`

This element wraps the set of rows that describe the table footers. It can be useful for displaying summaries, totals, or footnotes for the table's data.

### 5. `<tr>`

This element represents a table row. It wraps a set of table cells, which can be either header cells (`<th>`) or standard cells (`<td>`).

### 6. `<th>`

This element represents a header cell. By default, its content is bold and centered.

### 7. `<td>`

This element represents a standard table cell.

### 8. `<colgroup>` and `<col>`

These elements allow you to apply styles to an entire column (or a group of columns) at once.



## Instructor Activity | Code Implementation | Examples
```html
<table border="1">
    <!-- Table Header -->
    <thead>
        <tr>
            <th>Month</th>
            <th>Product A Sales ($)</th>
            <th>Product B Sales ($)</th>
            <th>Total Sales ($)</th>
        </tr>
    </thead>

    <!-- Table Body -->
    <tbody>
        <tr>
            <td>January</td>
            <td>1200</td>
            <td>800</td>
            <td>2000</td>
        </tr>
        <tr>
            <td>February</td>
            <td>1300</td>
            <td>850</td>
            <td>2150</td>
        </tr>
        <tr>
            <td>March</td>
            <td>1250</td>
            <td>900</td>
            <td>2150</td>
        </tr>
    </tbody>

    <!-- Table Footer -->
    <tfoot>
        <tr>
            <td>Total</td>
            <td>3750</td>
            <td>2550</td>
            <td>6300</td>
        </tr>
    </tfoot>
</table>

```

## Student Activities
Use MDN and create a table.


## Resources - Official Documentation and Other Resources
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form


---

# Interview questions

1. What are semantic tags?
2. Create a form in HTML for collecting user information. Perform form validation.