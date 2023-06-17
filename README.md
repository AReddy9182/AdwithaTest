# AdwithaTest
PART-A(Theory) Answers
1)Mention the working of Internet Website in terms of Front-end and Back-end Divisions.
Ans:- An internet website consists of two main divisions: the front-end and the back-end. Each division has its specific role and functionality in the overall 
functioning of a website.The term “front-end” refers to the user interface i.e users can interact directly with the website.Front-end developers design and 
construct the user experience elements on the web page or app including buttons, menus, pages, links, graphics and more.
 
 The primary technologies used in front-end development include HTML (Hypertext Markup Language), CSS (Cascading Style Sheets), and JavaScript. 
 a. HTML: HTML is used to structure the content of a website, defining the layout of the page and organizing different elements such as headings, paragraphs, 
 images, links, forms, and more.

b. CSS: CSS is responsible for the visual styling of the website, including colors, fonts, layouts, and overall appearance. It allows developers to control 
the presentation of HTML elements and create an appealing user interface.

c. JavaScript: JavaScript adds interactivity to the website, enabling dynamic elements, animations, form validation, and more. It allows developers to create a responsive
and engaging user experience.

d. Front-end Frameworks: Developers often use front-end frameworks like React, Angular, or Vue.js to simplify and streamline the development process. These frameworks
provide pre-built components, state management, and other tools for efficient front-end development.

Back-end:
The back-end is the server-side of a website that handles the behind-the-scenes operations and data processing. It includes the server, database, and server-side programming.
The core concern of back-end developers is in creating applications that can find and deliver data to the front end.

a. Server: The server hosts the website and responds to requests from users' browsers. It runs server-side software (e.g., Apache, Nginx) that manages the communication 
between the front-end and the back-end.

b. Database: The database stores and manages the website's data, including user information, content, and other relevant data. Common database systems include MySQL, 
PostgreSQL, MongoDB, etc.

c. Server-side Programming: Server-side programming languages (such as Python, PHP, Ruby, or Node.js) are used to handle the business logic and process user requests. 
They interact with the database, handle authentication, perform calculations, and generate dynamic content to be displayed on the front-end.

d. APIs (Application Programming Interfaces): APIs are used to facilitate communication and data exchange between the front-end and the back-end or between different 
systems. They allow developers to retrieve or send data in a standardized manner.

e. Back-end Frameworks: Back-end frameworks like Django (Python), Ruby on Rails (Ruby), or Laravel (PHP) provide a structured environment for building web applications 
efficiently. They offer libraries, tools, and conventions to simplify common back-end tasks.

Therefore the front end focuses on the presentation and user interface of a website, while the back end handles server-side processing, data management, and communication 
with the front end. Both divisions work together to deliver a functional, visually appealing, and interactive website to the users.


2) What are tags in HTML? Explain each category of tag with an Example.
   Ans:-  HTML tags are like keywords which defines how web browser will format and display the content. With the help of tags, a web browser can distinguish between HTML content and simple content. HTML tags contain three main parts: opening tag, content, and closing tag. But some HTML tags are unclosed tags.An HTML file must have some essential tags so that the web browser can differentiate between simple text and HTML text.

Here are some categories of HTML tags, along with examples for each category:
Structural Tags:
<html>: This tag represents the root element of an HTML page.
<head>: This tag contains meta-information about the document, such as the title, CSS stylesheets, or scripts.
<body>: This tag encloses the content of the web page that will be displayed in the browser.

 Heading Tags:
<h1> to <h6>: These tags are used to define headings of different levels. <h1> represents the highest level (main heading), and <h6> represents the lowest level (subheading).
 
Paragraph Tags:
<p>: This tag is used to define a paragraph of text.
 
 Formatting Tags:
<strong> or <b>: These tags are used to highlight text as bold.
<em> or <i>: These tags are used to emphasize text by italicizing it.

Hyperlink Tags:
<a href="https://example.com">: This tag creates a hyperlink and defines the URL (web address) to which the user will be directed when clicking on the link. The closing </a> tag signifies the end of the link.

Image Tags:
<img src="image.jpg" alt="Description">: This tag is used to insert an image into a web page. The src attribute specifies the image file's source (URL or file path), and the alt attribute provides alternative text that is displayed if the image cannot be loaded.

List Tags:
<ul>: This tag denotes an unordered list, typically rendered as bullet points.
<ol>: This tag denotes an ordered list, typically rendered with numbers or letters.
<li>: This tag defines an individual item within a list, placed within either <ul> or <ol> tags.

 Table Tags:
<table>: This tag represents a table structure in HTML.
<tr>: This tag defines a table row.
<th>: This tag defines a table header cell.
<td>: This tag defines a table data cell.
 
3) Explain the working Procedure of Virtual DOM.
 Ans:- The Virtual DOM (Document Object Model) is used to improve the efficiency and performance of updating the user interface (UI) of a web application which is used in web development such as React . The Virtual DOM works as an abstraction layer between the actual DOM and the application's components. 

Working Procedure of Virtual DOM:

Initial Rendering:

When an application using the Virtual DOM is first loaded, the initial rendering takes place. The component hierarchy is created, and the Virtual DOM is constructed as an in-memory representation of the actual DOM.
The Virtual DOM consists of lightweight JavaScript objects called "virtual elements" or "virtual nodes" that mirror the structure of the real DOM. These virtual nodes contain information about the corresponding real DOM nodes, such as tag names, attributes, and event handlers.

Component Update:

When a component's state or props change, triggering a re-render, the Virtual DOM comes into play.
The Virtual DOM performs a diffing algorithm, comparing the previous Virtual DOM state with the new state to identify the minimum number of changes required to update the UI efficiently.
The diffing algorithm analyzes the structural differences between the previous and new Virtual DOM trees, looking for added, removed, or modified virtual elements.

Creating a Patch:

Based on the diffing analysis, the Virtual DOM generates a patch, which is a set of instructions describing the necessary changes to be made to the real DOM.
The patch includes instructions like "add this node," "remove that node," or "update the text content of this node."
The patch is represented as a lightweight JavaScript object or data structure.

Applying the Patch:

Once the patch is generated, the Virtual DOM applies it to the real DOM to reflect the desired changes in the UI.
The patching process is optimized to minimize the number of operations required to update the real DOM, making it more efficient than directly manipulating the entire DOM tree.
The changes are selectively applied to the specific elements that need to be updated, rather than re-rendering the entire UI.
Reconciliation:

After the patch is applied to the real DOM, the process of reconciliation takes place. The Virtual DOM updates its internal representation to match the new state of the real DOM.
This ensures that subsequent updates can be efficiently compared against the updated Virtual DOM for future re-rendering cycles.

 
 Hence,this approach improves performance by minimizing the amount of work required to keep the UI in sync with the application's state, resulting in a more responsive and efficient user experience.


4) Mention some Differences between MySQL and No SQL
  Ans:-  MySQL and NoSQL (Not Only SQL) are both database management systems, but they have distinct differences in their data models, scalability, query languages, and use cases.
Some of the key differences between MySQL and No SQL:-

Data Model:

MySQL: MySQL is a relational database management system (RDBMS) based on the SQL (Structured Query Language) model. It organizes data into tables with predefined schemas, and relationships between tables are established using keys and foreign keys.
NoSQL: NoSQL databases use various data models, including key-value, document, columnar, and graph. They provide flexible schemas that allow for dynamic and schema-less data structures.

Scalability:

MySQL: MySQL follows a vertical scaling approach, where a single server is scaled up by adding more resources (CPU, memory, storage) to handle increased load. It is suitable for applications with moderate to high data volumes and read/write operations.
NoSQL: NoSQL databases are designed for horizontal scalability, also known as scaling out. They distribute data across multiple servers or nodes, enabling the database to handle high traffic and massive amounts of data. NoSQL databases are more suitable for large-scale, highly scalable applications.

Query Language:

MySQL: MySQL uses SQL as its query language. SQL is a standardized language for interacting with relational databases and supports powerful querying, filtering, joining, and aggregating operations.
NoSQL: NoSQL databases often have their own query languages or interfaces specific to the data model they use. Some NoSQL databases provide query capabilities similar to SQL, while others offer simpler CRUD (Create, Read, Update, Delete) operations or specialized query languages for specific use cases.

Schema Flexibility:

MySQL: MySQL enforces a rigid schema structure, requiring predefined table schemas with fixed columns and data types. Modifying the schema often involves altering the table structure, which can be a complex and time-consuming process.
NoSQL: NoSQL databases offer more flexibility with schema-less or dynamic schema models. They allow for storing and retrieving data without a predefined schema, enabling developers to adapt the database structure more easily as application requirements evolve.

Use Cases:

MySQL: MySQL is commonly used for traditional applications that require strong data consistency, complex querying, and transactional operations. It is well-suited for applications such as content management systems, e-commerce platforms, financial systems, and data-driven websites.
NoSQL: NoSQL databases excel in handling large amounts of unstructured or semi-structured data, providing high availability, horizontal scalability, and faster read/write operations. They are often used in real-time analytics, social media platforms, IoT (Internet of Things) applications, and situations where high scalability and performance a


5) Explain any one DBMS Technology in your own words.
   Ans:-  PostgreSQL is an open-source relational database management system that provides a powerful and feature-rich platform for managing and storing structured data. It is known for its robustness, scalability, and adherence to SQL standards. 

PostgreSQL follows the relational model of data management, where data is organized into tables with rows and columns.
It allows the definition of relationships between tables using primary keys, foreign keys, and constraints, ensuring data integrity and consistency.
SQL (Structured Query Language) is used to query, manipulate, and manage the data stored in PostgreSQL.

It offers a wide range of built-in data types, including numeric, character, date/time, JSON, arrays, and more. It also supports custom data types and allows users to define their own data type. It also supports extensibility through user-defined functions, operators, and data types, allowing developers to extend its functionality to meet specific requirements.

 PostgreSQL provides a rich set of SQL features, including complex joins, subqueries, window functions, and aggregate functions. It supports full-text search, regular expressions, and advanced indexing mechanisms.
It ensures ACID (Atomicity, Consistency, Isolation, Durability) properties, providing transactional integrity and reliability.

PostgreSQL has a large and active community of developers, contributors, and users, resulting in a vibrant ecosystem.It is cross-platform, meaning it can run on various operating systems, including Linux, Windows, macOS, and Unix-like systems.
It is available as a pre-compiled binary or can be built from source code to ensure compatibility with specific platforms.


PostgreSQL's combination of robustness, extensibility, and adherence to SQL standards makes it a popular choice for a wide range of applications. It is used in industries such as finance, telecommunications, e-commerce, scientific research, and more, where reliability, scalability, and data integrity are crucial.







