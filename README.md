# HTML-CSS-JS

___
> What is the purpose of the <!DOCTYPE> declaration in an HTML document?

The `<!DOCTYPE>` declaration is used to inform the browser which version of HTML or XHTML is being used in the document. It tells the browser how to interpret the elements and attributes in the document, and allows the browser to apply the correct rendering rules.

___
> Difference between html tag and element ?

___

> should we have more than one `<h1>` tag or not ?
**NO**, 
___

> what are the new thing introduced in html5 ?

HTML5 is the fifth version of HTML, the standard markup language used to create web pages. It introduces new features and improvements such as 
- semantic elements 
- multimedia support 
- offline storage and
- improved form controls. 

It also deprecates some older features and aims to improve the overall structure and accessibility of web pages.

___

> what do you mean by web accessibility ?

Web accessibility refers to the practice of designing and developing web content and applications that can be used by people with a wide range of abilities and disabilities. This includes individuals who may have visual, auditory, motor, cognitive or neurological impairments, as well as those who use assistive technologies such as screen readers, screen magnifiers, and alternative input devices.

Web accessibility is important because it ensures that everyone can access and use the web, regardless of their abilities. This includes people with disabilities, older adults, and users with low literacy or low-bandwidth connections.

To make a website accessible, developers should follow web accessibility guidelines such as the Web Content Accessibility Guidelines (WCAG) which are developed by the World Wide Web Consortium (W3C). These guidelines provide a set of best practices and standards for web accessibility, including guidelines for text, images, multimedia, and interactive elements.

Examples of web accessibility features include:

- Text alternatives for images, videos, and audio
- Keyboard-friendly navigation and controls
- High contrast colors for users with visual impairments
- Closed captioning for videos
- Simple and consistent layout, with clear headings and labels
- Clear and descriptive links

Web accessibility is an ongoing process, and it requires the involvement of developers, designers, content authors, and other stakeholders to ensure that accessibility is considered throughout the development process.

___

> difference between `display: inline-block` and `display: block` in css

`display: inline-block` and `display: block` are two different values for the display property in CSS that determine how an element is displayed on a web page.

`display: block:` When an element is set to display: block, **it takes up the full width of its parent container and creates a new block formatting context.** A block-level element will start on a new line and push any subsequent elements down. Block-level elements have a default width of 100% of their parent container and a default height that is determined by their content. Examples of block-level elements are div, h1, p, section.

`display: inline-block:` When an element is set to display: inline-block, it behaves like both an inline and a block-level element. **It takes up only as much width as necessary and does not create a new block formatting context.** An inline-block element will not start on a new line and will be placed next to any subsequent elements. Examples of inline-block elements are span, img, input.

The main difference between display: block and display: inline-block is that block elements take up the full width of their parent container and create a new block formatting context, while inline-block elements only take up as much width as necessary and do not create a new block formatting context.

It's important to keep in mind that display: inline-block has some quirks, such as the whitespace between inline-block elements creating unwanted gaps. You can use font-size:0 on the parent element to fix this problem, or you can use float property instead of display: inline-block which will avoid this problem.





___

> difference between `<svg>` & `<canvas>`?

___

> What is the difference between an `ID` and a `class` in HTML?

An ID is a unique identifier that can be used to target a specific element on a web page using CSS or JavaScript. An ID can be applied to only one element on a page, and it is defined using the id attribute. A class, on the other hand, can be applied to multiple elements on a page, and it is defined using the class attribute. Classes can be used to group elements together and apply styles or behavior to all elements in the group.


___

> RegEx ?


___

> How DOM is rendered in browser?

When a web page is loaded in a browser, the browser parses the HTML and CSS, and creates a Document Object Model (DOM) of the page. The DOM is a tree-like representation of the elements and their relationships in the HTML document.

The process of rendering a web page in the browser can be broken down into the following steps:

1. The browser receives the HTML and CSS from the server, and starts parsing the HTML to create the DOM. The browser reads the HTML tags and creates corresponding elements, such as div, span, and p, in the DOM.

2. As the browser parses the HTML, it also starts building the CSS Object Model (CSSOM) which is a representation of the styles applied to the elements in the DOM.

3. Once both the DOM and the CSSOM are created, the browser combines them to create the Render Tree. The Render Tree is a tree-like representation of the elements in the DOM that are visible and the styles that are applied to them.

4. Then, the browser starts layout process where it calculates the layout of each element in the Render Tree, such as the position, size, and visibility of each element. This step is also known as the "reflow" or "layout" phase.

5. Finally, the browser paints the elements in the Render Tree to the screen. This step is known as the "paint" phase.

The rendering process is an ongoing process, and the browser can re-render the page if the DOM or the styles change. The browser uses the browser's layout engine to calculate the layout of the elements on the page, and the process can be optimized using techniques such as lazy loading, using requestAnimationFrame, and avoiding unnecessary styles and elements.

Overall, the DOM, CSSOM and Render Tree work together to create the final visual representation of a web page that you see in the browser.

___

> Difference between async and differ attrubute in `<script>`

___

> what is responsive web design ?

___

> what is use of meta tags ?

___

> Difference between `attribute` and `property`?

In HTML, an attribute is used to provide additional information about an element, while a property is used to define the current state or value of an element.

An attribute is set on an HTML element using the HTML syntax, for example:
```html
<input type="text" value="Initial value">
```
A property, on the other hand, is a property of a JavaScript object that represents the element, and it can be accessed and modified using JavaScript. For example:
```js
let input = document.querySelector("input");
console.log(input.value); // Outputs: "Initial value"
input.value = "New value";
```
It's important to know that when an element is rendered by the browser, the values of the attributes are copied to the properties, so the attribute's initial value will be the same as the property's initial value. But after that, if you change the property's value, the attribute's value will not change.

For example, in the above example, the value of the value attribute and the value property will be the same initially, but if you change the value property using JavaScript, the value attribute will remain unchanged.

In summary, attributes provide metadata about an element and are defined in the HTML, while properties provide the current state of an element and can be accessed and modified using JavaScript.



___

> how iframe works?

___

> geoLoaction API ?

___

> do you optimize the performance of a web page?

Optimizing the performance of a web page can be done through a variety of techniques, including:
 - Minimizing the number of HTTP requests by combining and minifying files
 - Using a Content Delivery Network (CDN) to serve static assets
 - Using browser caching to store assets locally
 - Optimizing images and other media by compressing them and using the correct file format
 - Using lazy-loading to only load content as it is needed
 - Removing any unnecessary code or plugins
 - Optimizing JavaScript and CSS code for better load times

___

> 

___
> what do you mean by request life cycle ?

The request life cycle, also known as the request-response cycle, refers to the process that occurs between the time a client makes a request to a server and the time the server sends back a response. It typically includes the following steps:

 - **DNS Lookup:** The client's computer looks up the IP address of the server using the domain name of the website.

 - **TCP/IP Connection:** The client establishes a connection with the server using the Transmission Control Protocol (TCP) or the User Datagram Protocol (UDP).

 - **Request:** The client sends a request to the server, which includes information such as the URL, the HTTP method (e.g., GET, POST), and any data to be sent to the server.

 - **Server Processing:** The server receives the request and processes it. This may involve routing the request to the appropriate controller, executing any necessary business logic, and querying the database.

 - **Response:** The server sends a response back to the client, which may include the requested data, an error message, or a redirect.

 - **TCP/IP Close:** The client and server close the connection.

This process usually happens in milliseconds, and the client and server can handle multiple requests and responses simultaneously. The request life cycle is a fundamental concept in web development, and understanding it is essential for building and maintaining web applications.

It's important to note that the request life cycle is not limited to web application but also applies to other types of applications that involve client-server communication.

___

> what are symentic elements? and how they are useful?

Semantic markup is the practice of using HTML tags in a way that describes the meaning of the content, rather than its presentation. This is done by using appropriate HTML tags such as `<header>`, `<nav>`, `<article>`, `<section>`, `<aside>` and `<footer>` to indicate the different types of content on a web page, rather than using tags such as <div> and <span> that do not indicate the meaning of the content.

Here are some ways semantic markup can be useful:

  - **Accessibility:** Semantic markup makes it easier for assistive technologies, such as screen readers, to understand and navigate a web page. Assistive technologies rely on the HTML tags to understand the structure and meaning of the content, so using appropriate tags can greatly improve accessibility for users with disabilities.

  - **Search Engine Optimization (SEO):** Search engines use the HTML tags to understand the content and context of a web page. By using semantic markup, it can help search engines to better understand the content on the page and give it more context, which can improve the page's ranking in search engine results.

 - **Maintainability:** Semantic markup makes it easier for developers to understand and maintain a web page. By using clear and meaningful tags, it's easier to identify the purpose of different sections of the page, and it's also easier to make changes to the page without breaking the layout.

 - **Reusability:** Semantic markup allows for easy reusability of code. By providing clear and meaningful labels to the different sections of a web page, it's easy to copy and paste sections of code to another page or to a different website.

 - **Better CSS styling:** Semantic tags give more meaning to the HTML elements, making it easier to style them with CSS. With semantic tags, you can target specific sections of the page, rather than targeting individual elements with CSS selectors.

Overall, semantic markup is an important technique for building accessible, maintainable, and search engine friendly web pages.

___
> how does browser understand javascirpt ?
 
https://www.youtube.com/watch?v=2WJL19wDH68&list=PL_VYAa9CRontGgFvg1dSiTw1NlLa3CISy&index=12&ab_channel=AkshaySaini

When a browser loads a web page, it begins by parsing the HTML and creating a Document Object Model (DOM), which is a tree-like representation of the HTML elements and their relationships. Once the HTML has been parsed, the browser will then move on to parsing any JavaScript code that is present on the page.

The browser has a built-in JavaScript engine that is responsible for understanding and executing the JavaScript code. The most common JavaScript engines are V8 (used by Chrome and Edge), SpiderMonkey (used by Firefox), and JavaScriptCore (used by Safari).

When the JavaScript engine encounters a script tag, it will begin parsing the code and converting it into a format that the engine can understand. This process is called lexing and parsing. Once the code has been parsed, it will be executed by the engine.

The JavaScript engine uses a technique called just-in-time (JIT) compilation to speed up the execution of JavaScript code. The JIT compiler will analyze the code as it runs and optimize it for faster execution.

The JavaScript engine also provides a set of built-in objects and functions, such as the Math object and the console.log() function, that can be used by the JavaScript code. Additionally, the engine provides an interface to the DOM, which allows JavaScript code to interact with and manipulate the elements on the page.

Overall, the browser's JavaScript engine plays a crucial role in interpreting and executing JavaScript code, allowing web pages to be dynamic and interactive.
  
___
  
> what is prefetch, preload and preconnect in html?
  
`preconnect`, `preload` and `prefetch` are all resource hints that can be used to improve the loading performance of a web page by telling the browser to fetch resources in advance.

- preconnect: The preconnect hint tells the browser to open a connection to a specified resource in advance before the browser needs to use it. This can speed up the loading time by reducing the time it takes to establish a connection to the resource when it is needed.

 - preload: The preload hint tells the browser to fetch a specified resource as soon as possible, regardless of whether it is needed immediately or not. The resource is downloaded and made available for use, so that when it is needed, it can be used immediately without any delay.

 - prefetch: The prefetch hint tells the browser to fetch a specified resource in the background, and to store it in the cache. The resource is not used immediately, but it will be available for use if the user navigates to a page that needs that resource.

The main difference between them is when the browser should start fetching the resources, `preconnect` is used before the browser needs the resource, `preload` it used as soon as possible and `prefetch` is used when the browser is idle or when the user is expected to navigate to a specific resource.

It's important to note that not all browsers support these hints, and they might not work as expected in some cases. For example, using preload or prefetch on a resource that is not used can increase the load time.

Also, It's important to consider the user's network conditions, and device capabilities when using these hints.
  
___

> what is css specificity?
 
CSS specificity is a concept that determines which CSS styles will be applied to an HTML element. When multiple CSS styles are applied to the same element, the browser uses specificity to determine which styles should take precedence.

CSS specificity is calculated based on the combination of selectors used in the CSS rule. The more specific the selector is, the higher the specificity of the rule.

There are several types of selectors:

- **Inline styles:** These are styles that are applied directly to an HTML element using the style attribute. Inline styles have the highest specificity.

- **ID selectors:** These are styles that are applied to an HTML element based on its ID. ID selectors have a higher specificity than class selectors.

- **Class selectors, attribute selectors, and pseudo-class selectors:** These are styles that are applied to an HTML element based on its class, attribute, or pseudo-class. They have a lower specificity than ID selectors but higher than element selectors.

- **Element selectors:** These are styles that are applied to an HTML element based on its tag name. Element selectors have the lowest specificity.

When multiple styles are applied to the same element, the browser will apply the style with the highest specificity. If the specificity of two styles is the same, the style that appears later in the CSS will take precedence.

It's important to keep in mind that specificity is not always a straightforward concept, and it can be hard to predict which style will be applied to an element. Therefore, it's important to use clear and consistent naming conventions for CSS classes, and to keep the CSS as organized as possible.

 The !important declaration is used in CSS to make a style rule have higher specificity, and therefore take precedence over any other styles that may be applied to the same element.

You can use !important by adding it at the end of a CSS property value, like this:
 ```css
 /* Example of using !important */
p {
  color: blue !important;
}

 ```
 In the above example, the text color for all <p> elements will be blue, even if another style rule is used to set the text color to a different value.

It's important to note that the use of !important should be used sparingly and with caution, because it can make the CSS harder to maintain, and can cause unexpected behavior. The best practice is to use it only in cases where it's truly needed, and to make sure the specificity of selectors is used correctly.

It's also important to know that !important does not affect the cascading order of the CSS, but it only affects the cascading order between the selectors with the same specificity, the rule with the !important will always be applied.

It's highly recommended to avoid using !important in general.
___

> what are css selector and its rules?

 A CSS selector is a pattern used to select the HTML elements to which a set of CSS styles will be applied. There are several types of selectors in CSS, each with its own set of rules.

Here are some examples of common CSS selectors and their rules:

 - **Element Selector:** This selects elements based on their HTML tag name. For example, p will select all <p> elements.
 
```css 
p {
  /* styles here */
}
```
- **Class Selector:** This selects elements based on the value of their class attribute. For example, .myclass will select all elements with the class myclass.
 
 ```css
 .myclass {
  /* styles here */
}
 ```
 - **Id Selector:** This selects elements based on the value of their id attribute. For example, #myid will select the element with the id myid.
 
```css
 #myid {
  /* styles here */
}
 ```
 
- **Attribute Selector:** This selects elements based on the value of their attributes. For example, [href="https://example.com"] will select all elements that have an href attribute with the value https://example.com.
 
 ```css
 a[href="https://example.com"] {
  /* styles here */
}
 ```
 
- **Pseudo-class Selector:** This selects elements based on their state or position. For example, :hover will select an element when the user hovers over it.
 
```css
 a:hover {
  /* styles here */
}
```
 
- **Pseudo-element Selector:** This selects a specific part of an element. For example, ::before will select the content before the element.
 
```css
 p::before {
  /* styles here */
}
```
 
 It's also possible to chain selectors together to increase the specificity of a rule and make it more specific. For example, the following rule will select the <p> elements that are inside a <div> element with the class container.
 
 ```css
 div.container p {
  /* styles here */
}
```
 
 It's also possible to group selectors together, this way, the same styles can be applied to multiple selectors at once.
 
 > check this game https://frontend30.com/css-selectors-cheatsheet/
 
CSS allows you to combine selectors to target specific elements on a web page. This can be useful for creating more specific styles, or for applying styles to multiple elements at once.

Here are some examples of combining selectors:
 
- **Descendant Selector:** This is used to select elements that are descendants of a specific element. For example, the following CSS will select all <span> elements that are inside a <p> element:
 
 ```css
 p span {
  /* styles here */
}
```
 
- **Child Selector:** This is used to select elements that are direct children of a specific element. For example, the following CSS will select all `<li>` elements that are direct children of a `<ul>` element:
 
 ```css
 ul > li {
  /* styles here */
}
```
 
- **Adjacent Sibling Selector:** This is used to select elements that are directly after a specific element. For example, the following CSS will select all <p> elements that are directly after a `<h1>` element:
 
 ```css
 h1 + p {
  /* styles here */
}
```
 
- **General Sibling Selector:** This is used to select elements that are after a specific element (not necessarily directly). For example, the following CSS will select all `<p>` elements that are after a `<h1>` element:
 
```css
 h1 ~ p {
  /* styles here */
}
```
 
 In this example, all `<p>` elements that are after a `<h1>` element in the same parent element will be selected, regardless of the number of elements between them.

```html
 <div>
    <h1>Title</h1>
    <div>
        <p>This is a paragraph </p>
        <p>This is another paragraph </p>
    </div>
    <p>This is another paragraph </p>
    <p>This is one more paragraph </p>
</div>
```
 
In this example, the first and second `<p>` elements will be selected because they are after the `<h1>` element, but not the last one.

It's important to note that the General Sibling Selector is less specific than the Child Selector `(>)` and Adjacent Sibling Selector `(+)`, which means that it has lower precedence over other selectors.

___

> what is DRY Principle in javascript?

The DRY principle stands for "Don't Repeat Yourself" and it is a principle in software development that aims to minimize the amount of code duplication in a program. The idea behind DRY is that every piece of knowledge in the system should have a single, unambiguous representation.

In JavaScript, the DRY principle can be applied by using functions, variables, and objects to avoid repeating the same code multiple times. This can make the code more readable, maintainable, and less prone to errors.

Here are a few examples of how the DRY principle can be applied in JavaScript:

 1. **Functions:** Instead of repeating the same code multiple times, use a function that can be called whenever that code is needed.

 2. **Variables:** Instead of hard-coding values in multiple places, use variables to store the values and reference them throughout the code.

 3. **Objects:** Instead of repeating similar data structures, create an object that contains the data and methods for manipulating it.

 4. **Reusable modules:** Instead of writing similar functionality multiple times, modularize the code and reuse the modules.

Applying the DRY principle in JavaScript can help to make the code more concise, more organized, and more maintainable.

___

 > what are web workers ?

 Web Workers are a JavaScript API that allows you to run a script operation in a background thread separate from the main execution thread of a web page. This allows you to run expensive or time-consuming operations without freezing the user interface or blocking other scripts from running.

Web Workers communicate with the main thread by passing messages back and forth. The main thread can start a worker, pass it data, and receive results through the `postMessage()` method. The worker can also send data back to the main thread through the `postMessage()` method.

Web workers are useful for running time-consuming tasks such as image processing, complex calculations, or data manipulation without blocking the user interface. They can also be used to run background tasks, such as updating a database or sending data to a server, while the user continues to interact with the web page.

Web workers are supported by most modern browsers, but there are some limitations to their use, such as the inability to access the DOM and limitations on the types of API's that can be used within a worker.

Here is an example of how to create and use a web worker:
 ```js
 // Create a worker
const worker = new Worker('worker.js');

// Send data to the worker
worker.postMessage({data: 'Hello World'});

// Receive message from worker
worker.onmessage = function(e) {
  console.log(e.data);
}
 ```
 In worker.js:

```js
 // Receive data from the main thread
onmessage = function(e) {
  console.log(e.data);
  // Send message back to the main thread
  postMessage('Worker: ' + e.data);
}
```
 
 
___
 
> what is the output of code ?
 
```js
let a = true;

setTimeout(() => {
  a = false;
}, 2000);

while (a) {
  console.log("Hello World");
}
```
 
- The code will output "Hello World" indefinitely, as the while loop will continue to run until the value of `a` is set to false. However, the value of `a` will not be set to false until 2000 milliseconds (2 seconds) have passed due to the setTimeout function, so the loop will continue to run and print "Hello World" indefinitely.

___

> what is the output of code :
 
```js
[1, 2, 3, 4, 5].forEach((item) => {
  console.log(item);
  if (item === 2) {
    return;
  }
});
```

- The forEach method is used to iterate over each element of the array and call the provided function for each element. The function passed to forEach method has a parameter "item" which is the current element of the array. In this case, it will iterate over the array [1,2,3,4,5] and calls the function for each element. At each iteration, the current element is printed and then it checks if the current element is 2 and if it is true, it returns. But the `return` statement only exit the function, it doesn't stop the iteration. So it will print all the element of the array including 2.

___

