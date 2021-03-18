# Problem Domain, Objects, and the DOM

*A domain model is a system of abstractions that describes selected aspects of a sphere of knowledge, influence or activity. The model can then be used to solve problems related to that domain. The domain model is a representation of meaningful real-world concepts pertinent to the domain that need to be modeled in software. The concepts include the data involved in the business and rules the business uses in relation to that data. A domain model leverages natural language of the domain.*

*A domain model generally uses the vocabulary of the domain, thus allowing a representation of the model to be communicated to non-technical stakeholders. It should not refer to any technical implementations such as databases or software components that are being designed.*

### Problem Domain:

*Understanding the problem domain is the hardest part of programming.*

*Programming is easy if you understand the problem domain.*

*It is very difficult to solve a problem before you know the question. It’s like buzzing in on *Jeopardy before you hear the clue and shouting out random questions.*

*You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.*

### Objects:

*Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.*

### Programmers use a lot of name/value pairs:

1. HTML uses attribute names and values.
2. CSS uses property names and values.

### In JavaScript:

1. Variables have a name and you can assign them a value of a string, number, or Boolean.
2. Arrays have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)
3. Named functions have a name and value that is a set of statements to run if the function is called.
Objects consist of a set of name/value pairs (but the names are referred to as keys).
4. Literal notation is the easiest and most popular way to create opject.
Object

### The Document Object Model (DOM):

1. The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and tow.
2. how JavaScript can access and update the contents of a web page while it is in the browser window.
3. DOM trees have four types of nodes: document nodes, element nodes, attribute nodes and text nodes.
4. You can select element nodes by their id or clas attributes,by tag name, or using CSS selector syntax.
5. Whenever a DOM query can return more than one node, it will always return a nodelist.
6. In older browsers, implementation of the DOM is inconsistent(and is apopular reason for using jQuery).