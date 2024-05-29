### Question1 : Can you describe the different DOM traversal methods?

Solution:

1. Parent-Child Traversal: These methods allow navigation up and down the DOM tree between parent and child nodes. Example: firstChild, lastChild
2. Sibling Traversal: These methods allow navigation between sibling nodes at the same level in the DOM tree. Example: nextSibling, previousSibling
3. Ancestor Traversal: These methods allow navigation up the DOM tree from a given node to its ancestors. Example: closest
4. Traversal Utilities: These methods provide additional utilities for more complex traversal and manipulation of the DOM tree. Example: getElementsByTagName(tagName), getElementById(id)



### Question2: What are the levels involved in DOM?

Solution: 

- Level0: Provides a low-level set of interfaces.
- Level1: DOM level 1 can be described in two parts: CORE and HTML.
- Level2: consists of six specifications: CORE2, VIEWS, EVENTS, STYLE, TRAVERSAL, and RANGE.
- Level3: consists of five different specifications: CORE3, LOAD and SAVE, VALIDATION, EVENTS, and XPATH.
  

### Question3: What is MVC model?

Solution:

The Model-View-Controller (MVC) model is a design pattern used in software engineering to separate the concerns of an application into three interconnected components: the Model, the View, and the Controller. This separation helps organize code, making it more modular and easier to manage, test, and maintain.
- The Model represents the data and the business logic of the application
- The View is the user interface of the application.
- The Controller acts as an intermediary between the Model and the View. It processes user input, interacts with the Model, and updates the View.


### Question4: How can the style of an element be changed dynamically using DOM?

Solution : These methods provide different ways to dynamically change the style of an element using the DOM. The style property is straightforward for direct inline styles, while className and classList are useful for managing styles through CSS classes.


### Question5: How do you remove element from DOM?

Solution: These methods provide various ways to remove an element from the DOM:

- removeChild method: Used to remove a specific child from its parent.
- remove method: Called directly on the element to be removed.
- parentNode property: Used to access the parent and remove the child.
- innerHTML property: Used to clear the contents of a parent element.

### Question6: What is REST API?

Solution: A REST API provides a standardized way for different software applications to communicate with each other over the web using HTTP methods to perform CRUD operations on resources. It is stateless, resource-based, and usually formats data in JSON, making it a flexible and widely used approach for building web services.

### Question7: What is difference between map,filter and reduce?

Solution:

- Map: Transforms each element in an array. Returns a new array with transformed elements

- Filter: Returns a new array with elements that satisfy the condition. Filters elements in an array based on a condition.

- Reduce: Returns the single accumulated value. Reduces an array to a single value by applying a function.

### Question8: How do you stop event propagation?

Solution: BY using event.stopPropagation()

### Question9: What is CORS? 

Solution:CORS (Cross-Origin Resource Sharing) is a security feature implemented by web browsers to control how web applications interact with resources from different origins (domains). It is a mechanism that allows servers to specify who can access their resources and how these resources can be accessed.
- Access-Control-Allow-Origin: Specifies which origins are permitted to access the resource.
- Access-Control-Allow-Methods: Specifies which HTTP methods are allowed when accessing the resource.
- Access-Control-Allow-Headers: Specifies which HTTP headers can be used during the actual request.

### Question10: Explain the use of get and post method in REST APIS

Solution: GET and POST methods in REST APIs serve distinct purposes: GET is used for retrieving resources without causing side effects, while POST is used for creating new resources and potentially causing changes on the server.


