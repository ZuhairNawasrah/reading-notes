# JavaScript

## Object Literals

**Objects**: It group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names, **Variables** become **Properties**, and **Functions** become **Methods**.

There are several ways to create objects, **Literal notation** is the easiest and most popular way to create objects.

## Document Object Model

**Document Object Model** (DOM): specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

**Application Programming Interface** (API): let programs (and scripts) talk to each other.It's another name for DOM.

**DOM Tree**: A model of a web page that created by browser. It consists of four main types of nodes, which are:
1. **Document Node**: It represents the entire page.
2. **Element Node**: It describes the structure of an HTML page.
3. **Attribute Node**: It represents all attributes that carried within opening tags of HTML elements.
4. **Text Node**: It's the last child in the *DOM tree*, and cannot have children, just store the text inside *Element Node*. If an element contains text and another child element, that isn't child of *Text Node*, it's a child of that parent *Element Node*.

**DOM Queries**: Methods that find elements in the DOM tree. To store the result of any query, we must use variables, and by doing this we are storing location of the element in DOM tree in a variable. The properties and methods of that *element node* work on the variable.

There are two approaches to adding and removing content from a *DOM tree*, **innerHTML property** and **DOM manipulation**. DOM manipulation easily targets individual nodes in the DOM tree, whereas innerHTML is better suited to updating entire fragments.