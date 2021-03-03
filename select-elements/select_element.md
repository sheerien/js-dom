# How to select html element via js ?

## HTML Code

```html:
<div class="div-class">
  <div class="next-div-class">
    <h1 id="myID">Hello World</h1>
  </div>
</div>
```
## The methods by which I can select the element !?

### js code

```javascript:
// select element by id
var myID = document.getElementById("myID");
console.log(myID); // print h1 element in console screen

/*
Note : return single element have id attribute("myID")
*/
// select element by class name
var myClass = document.getElementsByClassName("div-class");
console.log(myClass); // print div own class = div-class in console screen
// OR
var mySecondClass = document.getElementsByClassName("next-div-class");
console.log(myClass); // print div own class = next-div-class in console screen

/*
Note 1: getElementsByClassName return => HTMLCollection == array 
Not 2: HTMLCollection don't have foreach method
*/
// select element by tag name
var myTag = document.getElementsByTagName("div");
console.log(myTag); // print all div elements for html page in console screen
// OR
var myTagH1 = document.getElementsByTagName("h1");
console.log(myTagH1); // print all h1 elements for html page in console screen

/*
Note 1: getElementsByTagName return => HTMLCollection == array 
Not 2: HTMLCollection don't have foreach method
*/

// select element by css selector
var mySelector = document.querySelector(".myClass");
console.log(mySelector); // print first element have class attribute(.myClass)
//OR
var myAllSelectors = document.querySelectorAll(".myClass");
console.log(myAllSelectors); // print All elements have class attribute("myClass")

/*
Note 1: querySelectorAll return => NodeList == array
Not 2: NodeList have foreach method
*/


/*
Note : Every element is a node but not every node is an element 
Because a node contains an HTML element and also contains node text etc ...
*/

```

## The properties by which I can select the element !?

### js code

```javascript:

// Property [ documentElement ]
var documentProp = document.documentElement;
console.log(firstProp); // print html for my page in console screen

// Property [ body ] & [ head ] & [ title ] & [ domain] & [ forms ] & [ images ] 
// property [ links ] & [ anchors ]

var bodyProp  = document.body;  console.log(bodyProp); 
var headProp  = document.head;  console.log(headProp);
var currentDomain = document.domain; console.log(currentDomain);
var formProp = document.forms; console.log(formProp); // return HTMLCollection
var imagesProp = document.images; console.log(imagesProp); // return HTMLCollection 
// Note: This property [images] is read-only 
var linksProp = document.links; console.log(linksProp); // return all element with href attribute only & return HTMLCollection
var anchorsProp = document.anchors; console.log(anchorsProp); // return all element with name attribute only & return HTMLCollection

/*
Note : All properties have it get and set but the properties read only have it only get
*/




```