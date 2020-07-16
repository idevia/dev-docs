# Guide for writing JavaScript code

## ECMAScript Standard

To prevent some errors caused by the quirky nature of JavaScript and to leverage its latest features, we have decided to only use the ECMAScript standard from ES6 onwards (Arrow functions, spread operators...yum 😋)

## Naming

Naming plays a very important role in coding. We have decided to use `camelCasing` for our variable and function names. We also want to avoid the use of special characters in our variable and function names.

Dos

?> **myAwesomeVariable**, **iLikeJs**, **variableName**, **myName2**

Don'ts

!> **my_awesome_variable**, **IlikeJS**, **variablename**, **_variableName**, **2myName**, **@#myName**

## Nesting

**One of the very important questions is should braces (`{` and `}`) have their own line or not?** Perfect answer does not exist for this question. It's all about personal preference. But to maintain consistency across our team, we have decided to not give them a separate line. Your code should look like:

```javascript
// if statements
if (condition) {
  // Code ...
} else {
  // Code ...
}

// For loops
for (...) {
  // Code
}

// Functions
myFunction = () => {
  // Your code here
}
```

Although it's mostly for consistency, there is one more reason we think braces should have their own line. Look at the following code block:

```javascript
function myName() {
  return
  {
    name: 'iDevia'
  }
}
```

JavaScript is a pretty quirky language, I think we can all agree on that. Upon calling the above function, you might not get what you are expecting. In fact, it will return nothing. This may produce unprecedented bugs in our apps, and also make them difficult to trace.

## Indentation

You must use **2 space** indentaion. Not a space more, not a space less.

```javascript
myFunction () => {
..// Your code
}
```

## Semi-colons

Modern JavaScript does not require semi-colons, so although you can add them, they are not necessary. We have decided to not use semi-colons at the end of lines in our projects and you are expected to do the same (or treat is imminent 😉).

```javascript
myFunction () => {
  const myName = 'iDevia'
  console.log(myName.toUpperCase())
}
```
## Quotes

For all the string variables and other such cases requiring the use of quotes, we have decided to use **single quotes**.