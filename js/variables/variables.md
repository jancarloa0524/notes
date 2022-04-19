# VARIABLES

The following declares a variable (when run this comes out as **undefined**):

``` javascript
var example;
```
[jsbin](https://jsbin.com/haginociwo/edit?js,console)

You can assign a value to a variable with the assignment operator, =, or an equal sign:

``` javascript
var example = ("value here");
```
[jsbin](https://jsbin.com/bavalanefu/edit?js,console)

Calculating with an undefined value will result in **NaN**:

``` javascript
var example = 1 + example;
```
[jsbin](https://jsbin.com/hahoxaluja/edit?js,console)

Characters put in between quotations marks are strings. The following is called a **string-literal**:

``` javascript
var example = "text here";
```
[jsbin](https://jsbin.com/kevefenuji/edit?js,console)

When you need a literal-quote inside a string, you need to use **back-slashes** like this:

``` javascript
var example = "text \"example\"."
```
[jsbin](https://jsbin.com/fojocitaho/edit?js,console)

You can use a " and ' in the same line, as shown by `ex4aSameString`. However, this becomes an issue when you are using the same character within the same line. The following shows an example of this, with a `ex4aGoodString` and `ex4aBadString`. Simply fix this with a backslash before the character:

``` javascript
var exampleSameString = ("John's car won't start")
var exampleGoodString = ('John\'s car won\'t start');
var exampleBadString = ('John's car wont' start);
```
[jsbin](https://jsbin.com/mekinaxase/edit?js,console)

You can do calculations within the decleration (+ , - , *, /):

``` javascript
var exampleAddition = 5 + 10;
var exampleSubtraction = 10 - 5;
var exampleMultiplication = 5 * 10;
var exampleDivision = 10 / 5;
```
[jsbin](https://jsbin.com/widehedibe/edit?js,console)

You can find the remainder using the % operator. For example, 5 divided by 2 would be equal to 2 with a remainder of 1 (2*2=4, 4+1=5):

``` javascript
var example = 5 % 2;
```
[jsbin](https://jsbin.com/retaceholo/edit?js,console)