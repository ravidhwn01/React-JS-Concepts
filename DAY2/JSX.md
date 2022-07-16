## Introduction to JSX

**Consider this variable declaration:**
```
const element = <h1>Hello, world!</h1>;
```
**This funny tag syntax is neither a string nor HTML.**

>>It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like.
>> JSX may remind you of a template language, but it comes with the full power of JavaScript.
JSX produces React “elements”


## Embedding Expressions in JSX
**In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:**
```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```

**You can put any valid JavaScript expression inside the curly braces in JSX.**
```
function formatName(user) {
  return user.firstName + ' ' + user.lastName;
}

const user = {
  firstName: 'Harper',
  lastName: 'Perez'
};

const element = (
  <h1>
    Hello, {formatName(user)}!
  </h1>
);
```
