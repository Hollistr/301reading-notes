# Class 301 Reading04

## React Docs - Forms

1. What is a ‘Controlled Component’?
    - React component that renders a form also controls what happens in that form on subsequent user input.

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
    - Store the response because the **name** attribute to each let the handler function choose what to do based on the value of event.target.name.

3. How do we target what the user is entering if we have an event handler on an input field?
    - event.target.namme

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?
    - To shorten your 'if' statements into one line of code with the conditional operator.

2. Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

**x===y ? true : false**

## Things I Want To Know More About

- More react, react, react!!!!

## Sources

- https://reactjs.org/docs/forms.html
- https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff
