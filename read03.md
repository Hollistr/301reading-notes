# Class 301 Reading03

## React Docs - lists and keys

1. What does .map() return?
    -.map() returns a new array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?
    - You loop using curly braces {}

3. Each list item needs a unique ____.
    - It needs its unique **keys**

4. What is the purpose of a key?
    - Keys help React identify which items have changed, are added, or are removed.

## The Spread Operator

1. What is the spread operator?
    - Spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

2. List 4 things that the spread operator can do.
    - Spread operators can copy an aray, use Math functions, add an item to a list, and combine objects.

3. Give an example of using the spread operator to combine two arrays.
    - const myArray = [`🤪`,`🐻`,`🎌`]
    const yourArray = [`🙂`,`🤗`,`🤩`]
    const ourArray = [...myArray,...yourArray]
    console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

4. Give an example of using the spread operator to add a new item to an array.
    - const fewFruit = ['🍏','🍊','🍌']
    const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

5. Give an example of using the spread operator to combine two objects into one.
    - const objectOne = {hello: "🤪"}
    const objectTwo = {world: "🐻"}
    const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
    console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
    const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
    objectFour.laugh() // 😂😂😂😂😂

## Things I Want To Know More About

- More react, react, react!!!