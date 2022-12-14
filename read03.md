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
    - Spread syntax refers to the use of an ellipsis of three dots (âĶ) to expand an iterable object into the list of arguments.

2. List 4 things that the spread operator can do.
    - Spread operators can copy an aray, use Math functions, add an item to a list, and combine objects.

3. Give an example of using the spread operator to combine two arrays.
    - const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
    const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
    const ourArray = [...myArray,...yourArray]
    console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ

4. Give an example of using the spread operator to add a new item to an array.
    - const fewFruit = ['ð','ð','ð']
    const fewMoreFruit = ['ð', 'ð', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]

5. Give an example of using the spread operator to combine two objects into one.
    - const objectOne = {hello: "ðĪŠ"}
    const objectTwo = {world: "ðŧ"}
    const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
    console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }
    const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("ð".repeat(5))}}
    objectFour.laugh() // ððððð

## Things I Want To Know More About

- More react, react, react!!!