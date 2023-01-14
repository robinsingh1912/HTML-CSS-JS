# HTML-CSS-JS

___
what is doctype?
- doctype 
___
what do you mean by request life cycle ?
- The request life cycle, also known as the request-response cycle, refers to the process that occurs between the time a client makes a request to a server and the time the server sends back a response. It typically includes the following steps:

**DNS Lookup:** The client's computer looks up the IP address of the server using the domain name of the website.

**TCP/IP Connection:** The client establishes a connection with the server using the Transmission Control Protocol (TCP) or the User Datagram Protocol (UDP).

**Request:** The client sends a request to the server, which includes information such as the URL, the HTTP method (e.g., GET, POST), and any data to be sent to the server.

**Server Processing:** The server receives the request and processes it. This may involve routing the request to the appropriate controller, executing any necessary business logic, and querying the database.

**Response:** The server sends a response back to the client, which may include the requested data, an error message, or a redirect.

**TCP/IP Close:** The client and server close the connection.

This process usually happens in milliseconds, and the client and server can handle multiple requests and responses simultaneously. The request life cycle is a fundamental concept in web development, and understanding it is essential for building and maintaining web applications.

It's important to note that the request life cycle is not limited to web application but also applies to other types of applications that involve client-server communication.

___

what are symentic elements? and how they are useful?
- Semantic markup is the practice of using HTML tags in a way that describes the meaning of the content, rather than its presentation. This is done by using appropriate HTML tags such as <header>, <nav>, <article>, <section>, <aside> and <footer> to indicate the different types of content on a web page, rather than using tags such as <div> and <span> that do not indicate the meaning of the content.

Here are some ways semantic markup can be useful:

 **Accessibility:** Semantic markup makes it easier for assistive technologies, such as screen readers, to understand and navigate a web page. Assistive technologies rely on the HTML tags to understand the structure and meaning of the content, so using appropriate tags can greatly improve accessibility for users with disabilities.

 **Search Engine Optimization (SEO):** Search engines use the HTML tags to understand the content and context of a web page. By using semantic markup, it can help search engines to better understand the content on the page and give it more context, which can improve the page's ranking in search engine results.

**Maintainability:** Semantic markup makes it easier for developers to understand and maintain a web page. By using clear and meaningful tags, it's easier to identify the purpose of different sections of the page, and it's also easier to make changes to the page without breaking the layout.
**
Reusability:** Semantic markup allows for easy reusability of code. By providing clear and meaningful labels to the different sections of a web page, it's easy to copy and paste sections of code to another page or to a different website.

**Better CSS styling:** Semantic tags give more meaning to the HTML elements, making it easier to style them with CSS. With semantic tags, you can target specific sections of the page, rather than targeting individual elements with CSS selectors.

Overall, semantic markup is an important technique for building accessible, maintainable, and search engine friendly web pages.





___

what is the output of code ?
```
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

what is the output of code :
```
[1, 2, 3, 4, 5].forEach((item) => {
  console.log(item);
  if (item === 2) {
    return;
  }
});
```
- The forEach method is used to iterate over each element of the array and call the provided function for each element. The function passed to forEach method has a parameter "item" which is the current element of the array. In this case, it will iterate over the array [1,2,3,4,5] and calls the function for each element. At each iteration, the current element is printed and then it checks if the current element is 2 and if it is true, it returns. But the `return` statement only exit the function, it doesn't stop the iteration. So it will print all the element of the array including 2.

___

