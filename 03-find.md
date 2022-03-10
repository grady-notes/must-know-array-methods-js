# Find => array.find()

Similar to the previous filter method, we have the find method which is also a condition based iteration method. The only difference is that the find method will return only single instance of the satisfied condition and this satisfied condition return will be an obejct. If no condition is satisfied the return will be `undefined` by default, but if the condition is satisfied multiple times, only the first satisfied condition will be returned.

A functional approach of the find method is shown below

```javascript
let people = [
    { name: "Grady", pos: "Developer" },
    { name: "Another Grady", pos: "Developer" },
    { name: "Raymond", pos: "Ethical Hacker" },
    { name: "Aatif", pos: "Coder" }
]

const get = (arr, pos) => {
    let found = arr.find((item) => {
        if (item.pos == pos) return item
        return false
    })
    return found
}

console.log(get(people, "Developer"));
```

**Note that there are 2 entries as developer which means that the condition is satisfied multiple times. but the output will contain only one instance which is the first satisfied condition among all others.**

[Previous : Filter Method](02-filter.md) | [Next : Reduce Method](04-reduce.md)
