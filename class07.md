# Domain model

*A domain model is a system of abstractions that describes selected aspects of a sphere of knowledge, influence or activity (a domain[3]). The model can then be used to solve problems related to that domain. The domain model is a representation of meaningful real-world concepts pertinent to the domain that need to be modeled in software. The concepts include the data involved in the business and rules the business uses in relation to that data. A domain model leverages natural language of the domain.*

*A domain model generally uses the vocabulary of the domain, thus allowing a representation of the model to be communicated to non-technical stakeholders. It should not refer to any technical implementations such as databases or software components that are being designed.*

*In software engineering, a domain model is a conceptual model of the domain[definition needed] that incorporates both behavior and data. In ontology engineering, a domain model is a formal representation of a knowledge domain with concepts, roles, datatypes, individuals, and rules, typically grounded in a description logic.*

*A domain model is generally implemented as an object model within a layer that uses a lower-level layer for persistence and "publishes" an API to a higher-level layer to gain access to the data and behavior of the model.*

*In the Unified Modeling Language (UML), a class diagram is used to represent the domain model.*

# Tables

## What's a Table?

*A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.*

*Grids allow us to understand complex data by referencing information on two axes.*

*Each block in the grid is referred to as a table cell. In HTML a table is written out row by row.*

*There are several types of information that need to be displayed in a grid or table. For example: sports results, stock reports, train timetables.*

*When representing information in a table, you need to think in terms of a grid made up of rows and columns (a bit like a spreadsheet). In this chapter you will learn how to:*

1. Use the four key elements for creating tables.
2. Represent complex data using tables.
3. Add captions to tables.

## Basic Table Structure

### <table>

*The <table> element is used to create a table. The contents of the table are written out row by row.*

### <tr>

*You indicate the start of each row using the opening <tr> tag. (The tr stands for table row.) It is followed by one or more <td> elements (one for each cell in that row). At the end of the row you use a 
closing </tr> tag.*

### <td>

*Each cell of a table is represented using a <td>element. (The td stands for table data.)At the end of each cell you use a closing </td> tag.*

## Table Headings

### <th>

*The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading).*

*Even if a cell has no content, you should still use a <td> or <th> element to represent the presence of an empty cell otherwise the table will not render correctly. (The first cell in the first row of this example shows an empty cell).*

*Using <th> elements for headings helps people who use screen readers, improves the ability for search engines to index your pages, and also enables you to control the appearance of tables better when you start to use CSS.*

*You can use the scope attribute on the <th> element to indicate whether it is a heading for a column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column.*

## Spanning Columns

*Sometimes you may need the entries in a table to stretch across more than one column.*

*The colspan attribute can be used on a <th> or <td> element and indicates how many columns that cell should run across.*

*In the example on the right you can see a timetable with five columns; the first column contains the heading for that row (the day), the remaining four represent one hour time slots.*

*If you look at the table cell that contains the words 'Geography' you will see that the value of the 
colspan attribute is 2, which indicates that the cell should run across two columns. In the third row, 'Gym' runs across three columns.*

*You can see that the second and third rows have fewer <td> elements than there are columns. This is because, when a cell extends across more than one column, the <td> or <th>cells that would have been in the place of the wider cells are not included in the code.*

## Spanning Rows

*You may also need entries in a table to stretch down across more than one row.*

*The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell should span down the table.*

*In the example on the left you can see that ABC is showing a movie from 6pm - 8pm, whereas the BBC and CNN channels are both showing two programs during this time period (each of which lasts one hour).*

*If you look at the last <tr>element, it only contains three elements even though there are four columns in the result below. This is because the movie in the <tr> element above it uses the rowspan attribute to stretch down and take over the cell below.*

## Long Tables

*There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).*

*These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table (as you will see when you learn about CSS).*

### <thead>

*The headings of the table should sit inside the <thead> element.*

### <tbody>

*The body should sit inside the <tbody> element.*

### <tfoot>

*The footer belongs inside the <tfoot> element.*

*Some of the HTML editors that come in content management systems offer tools to help draw tables. If the first row of your table only contains <th>elements then you may find that the editor inserts a <thead>element automatically.*

*Part of the reason for having separate <thead> and <tfoot>
elements is so that, if you have a table that is taller than the screen (or, if printed, longer than one page) then the browser can keep the header and footer visible whilst the contents of the table scroll. This is intended to make it easier for users to see which column the data is in (however this functionality is not implemented by default in any current browser).*

## Old Code:

### Width & Spacing

*There are some outdated attributes which you should not use on new websites. You may, however, come across some of them when looking at older code, so I will mention them here. All of these attributes have been replaced by the use of CSS.*

*The width attribute was used on the opening <table> tag to indicate how wide that table should be and on some opening <th> and <td> tags to specify the width of individual cells. The value of this attribute is the width of the table or cell in pixels.*

*The columns in a table need to form a straight line, so you often only see the width attribute on the first row (and all subsequent rows would use that setting).*

*The opening <table> tag could also use the cellpaddingattribute to add space inside each cell of the table, and the cellspacing attribute to create space between each cell of the table. The values for these attributes were given in pixels.*

### Border & Background

*The border attribute was used on both the <table> and <td>elements to indicate the width of the border in pixels.*

*The bgcolor attribute was used to indicate background colors of either the entire table or individual table cells. The value is usually a hex code (which we discuss on pages 249-252).*

*This example uses the HTML border and bgcolor attributes. No CSS attributes were utilized in this example.*

*When building a new website you should use CSS to control the appearance of the table rather than these attributes. They are only covered here because you may come across them if you look at the code of older websites.*

# Functions

*A typical use of a function object is in writing callback functions. A callback in procedural languages, such as C, may be performed by using function pointers.[2] However it can be difficult or awkward to pass a state into or out of the callback function. This restriction also inhibits more dynamic behavior of the function. A function object solves those problems since the function is really a façade for a full object, carrying its own state.*

*n JavaScript, functions are first class objects. JavaScript also supports closures.Compare the following with the subsequent Python example.*

#### example:

*function Accumulator(start) {
  var current = start;
  return function (x) {
    return current += x;
  };
}
An example of this in use:

var a = Accumulator(4);
var x = a(5);   // x has value 9
x = a(2);       // x has value 11

var b = Accumulator(42);
x = b(7);       // x has value 49 (current = 49 in closure b)
x = a(7);       // x has value 18 (current = 18 in closure a)*

# Method (computer programming)

*A method in object-oriented programming (OOP) is a procedure associated with a message and an object. An object consists of data and behavior; these comprise an interface, which specifies how the object may be utilized by any of its various consumers.*

*Data is represented as properties of the object, and behaviors are represented as methods. For example, a Window object could have methods such as open and close, while its state (whether it is open or closed at any given point in time) would be a property.*

*In class-based programming, methods are defined in a class, and objects are instances of a given class. One of the most important capabilities that a method provides is method overriding - the same name (e.g., area) can be used for multiple different kinds of classes. This allows the sending objects to invoke behaviors and to delegate the implementation of those behaviors to the receiving object. A method in Java programming sets the behavior of a class object. For example, an object can send an area message to another object and the appropriate formula is invoked whether the receiving object is a rectangle, circle, triangle, etc.*

*Methods also provide the interface that other classes use to access and modify the properties of an object; this is known as encapsulation. Encapsulation and overriding are the two primary distinguishing features between methods and procedure calls.*

### Type of methods:

1. Method overriding:

*and overloading are two of the most significant ways that a method differs from a conventional procedure or function call. Overriding refers to a subclass redefining the implementation of a method of its superclass. For example, findArea may be a method defined on a shape class. The various subclasses: rectangle, circle, triangle, etc. would each define the appropriate formula to calculate their area. The idea is to look at objects as "black boxes" so that changes to the internals of the object can be made with minimal impact on the other objects that use it. This is known as encapsulation and is meant to make code easier to maintain and re-use.*

2. Method overloading:

*on the other hand, refers to differentiating the code used to handle a message based on the parameters of the method. If one views the receiving object as the first parameter in any method then overriding is just a special case of overloading where the selection is based only on the first argument. The following simple Java example illustrates the difference*

# Object

*In computer science, an object can be a variable, a data structure, a function, or a method, and as such, is a value in memory referenced by an identifier.*

*In the object-oriented programming paradigm object can be a combination of variables, functions, and data structures; in particular in class-based variation of the paradigm it refers to a particular instance of a class.*

*In the relational model of database management, an object can be a table or column, or an association between data and a database entity (such as relating a person's age to a specific person).*

### Object-based languages

*An important distinction in programming languages is the difference between an object-oriented language and an object-based language. A language is usually considered object-based if it includes the basic capabilities for an object: identity, properties, and attributes. A language is considered object-oriented if it is object-based and also has the capability of polymorphism, inheritance, encapsulation, and, possibly, composition. Polymorphism refers to the ability to overload the name of a function with multiple behaviors based on which object(s) are passed to it. Conventional message passing discriminates only on the first object and considers that to be "sending a message" to that object. However, some OOP languages such as Flavors and the Common Lisp Object System (CLOS) enable discriminating on more than the first parameter of the function.[2] Inheritance is the ability to subclass an object class, to create a new class that is a subclass of an existing one and inherits all the data constraints and behaviors of its parents but also adds new and/or changes one or more of them.*

### Object-oriented programming

*Object-oriented programming is an approach to designing modular reusable software systems. The object-oriented approach is an evolution of good design practices that go back to the very beginning of computer programming. Object-orientation is simply the logical extension of older techniques such as structured programming and abstract data types. An object is an abstract data type with the addition of polymorphism and inheritance.*

*Rather than structure programs as code and data, an object-oriented system integrates the two using the concept of an "object". An object has state (data) and behavior (code). Objects can correspond to things found in the real world. So for example, a graphics program will have objects such as circle, square, menu. An online shopping system will have objects such as shopping cart, customer, product. The shopping system will support behaviors such as place order, make payment, and offer discount. The objects are designed as class hierarchies. So for example with the shopping system there might be high level classes such as electronics product, kitchen product, and book. There may be further refinements for example under electronic products: CD Player, DVD player, etc. These classes and subclasses correspond to sets and subsets in mathematical logic.*

### Distributed objects

*The object-oriented approach is not just a programming model. It can be used equally well as an interface definition language for distributed systems. The objects in a distributed computing model tend to be larger grained, longer lasting, and more service-oriented than programming objects.*

*A standard method to package distributed objects is via an Interface Definition Language (IDL). An IDL shields the client of all of the details of the distributed server object. Details such as which computer the object resides on, what programming language it uses, what operating system, and other platform-specific issues. The IDL is also usually part of a distributed environment that provides services such as transactions and persistence to all objects in a uniform manner. Two of the most popular standards for distributed objects are the Object Management Group's CORBA standard and Microsoft's DCOM.*