1.What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Answer: 
getElementById(): To find one element by its special ID name.Since IDs are unique,it always returns just one element.
Example:document.getElementById("box").

getElementsByClassName(): To find all elements that share the same class name.It returns a collection  of elements.
Example:document.getElementsByClassName("item").

querySelector(): Uses CSS-style selectors to find elements.It returns only the first matching element it finds.
Example:document.querySelector("button");

querySelectorAll(): It also uses CSS selectors but returns all matching elements as a collection.
Example:document.querySelectorAll(".card")

2.How do you create and insert a new element into the DOM?
Answer: At first we have to Use document.createElement() to create new element.Then we have to add text or content using innerText or innerHtml.We need to find the parent element where we want to insert it using method like getElementById or querySelector.Finally insert the new element into the DOM using appendChild() or insertBefore().

3.What is Event Bubbling and how does it work?
Answer:Event Bubbling is a process in the DOM where an event starts from the target element which is clicked and then moves upward to its parent,then to the parent’s parent and continues until it reaches the document root.This means parent elements can also respond to events that happen on their children.

4.What is Event Delegation in JavaScript?Why is it useful? 
Answer:Event Delegation is a method in JavaScript where we put an event listener on a parent element to handle events on its child elements.It is useful because we don’t need to add events to every child,which saves code and works faster when there are many children.
It also saves memory,works for new element and easier to manage.

5.What is the difference between preventDefault() and stopPropagation() methods?
Answer:These two methods are used to control events.

preventDefault():It stops the normal behavior of an element.For example,it can prevent a link from opening a new page or a form from refreshing the page.

stopPropagation():It stops the event from bubbling up to parent elements.Other elements won't know the event happened.
