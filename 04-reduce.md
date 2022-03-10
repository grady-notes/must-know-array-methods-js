# Reduce => array.reduce()

Reduce is one of the more complicated iteration methods of an array which requires a callback to work with. The key difference between the previous methods and the reduce method is that the previous methods return an entirely new array, whereas the reduce method reduces the initial / original / main array to a single value which can be any single data type (single number, single object, single array, etc)

Reduce method callback requires 2 parameters. One being the total number of calculations that are to be done in the current block generally known as the accumulator and the second one being the current iteration pointer or `this` value.

The reduce method itself takes 2 parameters, one being the above mentioned callback and the second one being the total initial value known as initiator. Generally the initiator is set to `0` which increases as the loop proceeds.

An example of reduce method is shown below by adding the daily salaries of employees :

```javascript
let people = [
    { name: "Grady", salary: 100 },
    { name: "Raymond", salary: 200 },
    { name: "Oliver", salary: 300 }
]

const dailyTotalOf = (arr) => {
    let reduced = arr.reduce((total, person) => {
        total += person.salary
        return total;
    }, 0)
    console.log(reduced)
}

dailyTotalOf(people)

// this will add all the salaries and return a single value instead of a new array
```

[Previous : Find Method](03-find.md)
