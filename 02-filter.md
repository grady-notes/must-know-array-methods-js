# Filter => array.filter()

Similar to the previous map method, the filter method method also iterates over a anarray and returns a new one. The only difference is that the size of this newly returned array can be maniplated with some or the other conditional statements. 

An example showing the functional approach of the `filter` method is shown below :

```javascript
let people = [
    { name: "Grady", pos: "Developer" },
    { name: "Raymond", pos: "Ethical Hacker" },
    { name: "Aatif", pos: "Coder" }
]

const get = (arr, pos) => {
    let filtered = arr.filter((item) => {
        if (item.pos == pos) return item
        return false
    })
    return filtered
}

console.log(get(people, "Developer"));
```

[Previous : Map Method](01-map.md) | [Next : Find Method](03-find.md)
