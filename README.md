# HTML-CSS-JS

___
> what is doctype?
- doctype 
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
 
 - **Child Selector:** This is used to select elements that are direct children of a specific element. For example, the following CSS will select all <li> elements that are direct children of a <ul> element:
 
 ```css
 ul > li {
  /* styles here */
}
```
 
 - **Adjacent Sibling Selector:** This is used to select elements that are directly after a specific element. For example, the following CSS will select all <p> elements that are directly after a <h1> element:
 
 ```css
 h1 + p {
  /* styles here */
}
```
 
 - **General Sibling Selector:** This is used to select elements that are after a specific element (not necessarily directly). For example, the following CSS will select all <p> elements that are after a <h1> element:
 
```css
 h1 ~ p {
  /* styles here */
}
```
 
 In this example, all <p> elements that are after a <h1> element in the same parent element will be selected, regardless of the number of elements between them.

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
 
In this example, the first and second <p> elements will be selected because they are after the <h1> element, but not the last one.

It's important to note that the General Sibling Selector is less specific than the Child Selector (>) and Adjacent Sibling Selector (+), which means that it has lower precedence over other selectors.

___

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

