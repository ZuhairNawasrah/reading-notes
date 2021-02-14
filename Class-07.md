# Object-Oriented Programming, HTML Tables

## Domain Modeling

**Domain Modeling**: Is the process of creating a conceptual model in code for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem. Here's some tips to follow when building your own domain models:

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the `new` keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the `this` variable within methods so you can access the object's properties and methods from inside.

## Objects

To create a new object, it's similar to define a new array, the only difference is we open curly braces `{}` instead of square bracts `[]`, e.g:
- `const objName = {key1:value1, key2:value2,.....}`

To update the value of properties, there are two methods, by using dot notation or using square brackets. They work on either objects created using literal or using constructor notation.To delete a property, just use the `delete` keyword, e.g:
- `this.propertyName = newValue ;`........Updating the value.
- `delete this.propertyName ;`.........Deleting the whole property.

`this` is a keyword that commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.