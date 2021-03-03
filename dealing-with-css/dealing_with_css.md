# Dealing with CSS 

```html:
<div>
    <h1 id="myID">Dealing with css</h1>
</div>

```

## JS Code

```javascript:
// select element by id
var myTagID = document.getElementByID("myID");
// property css in js dom [style]
/*
Note : The property is written in css => background-color [ cbab-case ]
As for JavaScript, it is written this way => backgroundColor [camelCase]
*/

// set value for style property
myTagID.style.backgroundColor = '#080';
/*
Note : style property => deal with only inline style 
As for dealing with the external style, we use the property [

    console.log(window .getComputedStyle(myTagID).backgroundColor);
]
*/
```