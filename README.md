# HTML-CSS-JS

what is doctype?
-

what are symentic elements?
- Semantic HTML elements are those that clearly describe their meaning in a human- and machine-readable way.

> The semantic elements added in HTML5 are:
 `<article>` , `<aside>` , `<footer>`, `<header>`, `<nav>`, `<main>`, `<section>`


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
