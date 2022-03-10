# Map => array.map()

Map method of Javascript is used to map the contents of one array into another. Map method takes one callback function as an argument and this callback takes an event that will be manipulated and stored into the new array. The callback function returns the map value using the `return` keyword.

An example of squaring the values of one array and storing them into another using the map method is shown below :

```javascript
let arr = [1,2,3];
let mapped = arr.map((item) => {
    return item * item;
});
console.log("original : ", arr);
console.log("mapped : ", mapped);
```

This was the simplest possible demonstration of map method. A more realistic example of iterating over an object array is shown below (map method is used in combination with function, to demonstrate in a more realistic way) :

```javascript
let people = [
    {name: "grady", age: 19},
    {name: "raymond", age: 21},
    {name: "someone else", age: 69},
];
const displayInfoOf = (arr) => {
    arr.map((person) => {
        // here the event variable is named as person, however it can be named anything related to the function so that everything makes sense
        console.log(`
            Name: ${person.name},
            Age: ${person.age}
        `);
    });
};
displayInfoOf(people);
```

[Next : Filter Method](02-filter.md)
