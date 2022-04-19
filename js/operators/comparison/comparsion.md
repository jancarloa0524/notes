# Comparison Operators

**Equality Operator:** A comparison operator that checks if two values are equivalent; a boolean. It attempts to convert both values being compared to a common type.
``` javascript
function example(val) {
    if (val == 10) {
        console.log(val + " is equal to 10")
    } else {
        console.log(val + " is not equal to 10")
    }
}

example(10);
example("10");
example(20);
```
[jsbin]()

**Strict Equality Operator:** A comparison operator that also checks if two values are equivalent; a boolean. A strict equality operator that does not perform any conversion
``` javascript
function example(val) {
    if (val === 10) {
        console.log(val + " is equal to 10")
    } else {
        console.log(val + " is not equal to 10")
    }
}

example(10);
```
[jsbin]()

**Inequality Operator:** Is the opposite of the equality operator; a boolean. Would return true if actually false, and vice versa. 
``` javascript
function example(val) {
    if (val != 10) {
        console.log(val + " is not equal to 10")
    } else {
        console.log (val + ' is equal to 10')
    }
}

example(20);
// The following, for some reason, won't work but it does in jsbin
ex20c("10");
ex20c(10);
```
[jsbin]()

**Strict Inequality Operator:** Same as the inequality operator; a boolean. Will not convert data types. 
``` javascript
function ex20c(val) {
    if (val !== 10) {
        console.log(val + " is not equal to 10")
    } else {
        console.log (val + ' is equal to 10')
    }
}

ex20c(10);
// The following is a string
ex20c("10");
```
[jsbin]()

**Greater Than Operator:** a boolean. Checks to see if a value is greater than another. 
``` javascript
function ex20e(val) {
    if (val > 10) {
        console.log(val + " is greater than 10")
    } else {
        console.log(val + " is not greater than 10")
    }
}

ex20e(11)
ex20e(9)
```
[jsbin]()

**Greater Than or Equal to Operator:** a boolean. Same as before, but also checks if it is equal. 
``` javascript
function ex20f(val) {
    if (val >= 10) {
        console.log(val + " is greater than/equal to 10")
    } else {
        console.log(val + " is not greater than/equal to 10")
    }
} 

ex20f(10)
ex20f(11)
ex20f(9)
```
[jsbin]()

**Less Than Operator:** a boolean. Checks to see if a value is less than another. 
``` javascript
function ex20g(val) {
    if(val < 10) {
        console.log(val + " is less than 10")
    } else {
        console.log(val + " is not less than 10")
    }
}

ex20g(9)
ex20g(11)
```
[jsbin]()

**Less Than or Equal to Operator:** a boolean. Same as before, but also checks if it is equal. 
``` javascript
function ex20h(val) {
    if(val <= 10) {
        console.log(val + " is less than/equal to 10")
    } else {
        console.log(val + " is not less than 10")
    }
}

ex20h(9)
ex20h(10)
ex20h(11)
```
[jsbin]()

**Logical And Operator:** a boolean. Only returns true if both values on the left and right are true.
``` javascript
function ex20i(val) {
    if (val > 10 && val < 20) {
        console.log(val + " is greater then 10, and less than 20")
    } else {
        console.log(val + " is not greater then 10, and not less than 20")
    }
}

ex20i(15)
ex20i(5)
```
[jsbin]()

**Logical Or operator:** a boolean. Only returns true if either of the operands is true.
``` javascript
function ex20j(val) {
    if (val > 20 || val < 10) {
        console.log(val + " is greater then 20, or less than 10")
    } else {
        console.log(val + " is not greater then 20, or not less than 10")
    }
}

ex20j(15)
ex20j(5)
```
[jsbin]()

`typeof` Returns the type of variable/value.
``` javascript
var num = 20
var string = "20"
console.log(typeof int)
console.log(typeof string)
```
[jsbin]()
