# Selector and Changing HTML

document.querySelector (query is like a question) finds something in a document, such as an HTML element.
``` javascript
var myh1 = docuemnt.querySelector('h1')
```

Classes and ID's in CSS, require their selectors when called by the DOM. CSS SYNTAX ONLY, NO HTML SYNTAX
``` javascript
var id = document.querySelector('#id')
var class = document.querySelector('.class')
```
[jsbin]() (Set this to all the above)

--Above examples are SAVING values to variables--

To select innner HTML, you need to use `.innerHTML`, while calling another saved variable from earlier
``` javascript
console.log('myh1.innerHTML')
```

You can also write/add to the inner HTML
``` javascript
// For now, lets say that the inner HTML for h1 is <h1>Heading</h1>
myh1.innerHTML = 'Title' // Changes it from <h1>Heading</h1> to <h1>Title</h1>. THE DOCUMENT ITSELF DOES NOT CHANGE
myh1.innerHTML += ' Card' // Adds ' Card' to set h1 to <h1>Title Card</h1>
```
[jsbin]() (Set this to all the above)

You can select parts of an element such as the `href` or `src` and change it's value with DOM
`.attributeName`
    `select an attribute of an element`

``` html
<a href="page_link">here</a>?</p>
<img src="image_link">
```
``` javascript
document.querySelector('a').href = "link";
document.querySelector('img').src = "link";
```

Extra cool thing: you can concatenate the link, so instead of setting the link to a website to something new, if its in the same website, for example. `hstat.org`, and you want your link to now go to `hstat.org/academics`, then instead do `.href += "academcis"`

[jsbin]() (Set this to all the above)