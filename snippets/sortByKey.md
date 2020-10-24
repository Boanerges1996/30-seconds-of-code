---
title: sortByKey
tags: array, function, intermediate
---

Return array of sorted objects by key

- Given an array of objects and key, sort the array by the provided key objects.
- Uses `Array.prototype.sort()` to sort by comparing the various keys the between object in array.

```js
const sortByKey = (array, key) =>
  array.sort((a, b) => (a[key] < b[key] ? -1 : a[key] > b[key] ? 1 : 0));
```

```js
const data = [
  {
    name: "Samson Kwaku",
    age: 22,
  },
  {
    name: "Boanerges Nkrumah",
    age: 18,
  },
];

sortByKey(data, "age"); // [{name:"Boanerges Nkrumah,age:18},{name:"Samson Kwaku",age:22}]
```
