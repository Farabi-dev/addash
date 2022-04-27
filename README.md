# Addash

addash is a library like lodash. I am creating the library on my way. Anyone can use this library. I will try to create all the features as lodash does. Brief description of all features are given below:

=> **chunk(arr, size)**  
Split an array into groups the length of size. Remaining elements are stored in a new array.

- arguments: arr(Array), size(number)
- returns: Array

Example:

```js
chunk(['a', 'b', 'c', 'd'], 2); // [['a', 'b'], ['c', 'd']]
chunk(['a', 'b', 'c', 'd'], 3); // [['a', 'b', 'c'], ['d']]
chunk(['a', 'b', 'c', 'd'], 5); // []
chunk(['a', 'b', 'c', 'd'], -5); // []
chunk([], 3); // []
```

=> **compact(arr)**  
Filter an array with only truthy values.

- arguments: arr(Array)
- returns: Array

Example:

```js
compact([0, 1, false, 2, '', 3]); // [1, 2, 3]
compact([0, 1, true, 'text', null, undefined, NaN, false, 2, '', 3]); // [1, true, 'text', 2, 3]
```

=> **concat(arr, ...values)**  
Creates an array by concatenating with more arrays or values.

- arguments: arr(Array, ...values)
- returns: Array

Example:

```js
concat([1], 2, [3], [[4]]); // [1, 2, 3, [4]]
concat(1, 2, [3], [[4]]); // []
concat(); // []
```

=> **difference(arr, [values])**  
Creates an array by concatenating with more arrays or values.

- arguments: arr(Array, [values])
- returns: Array

Example:

```js
difference([2, 1], [2, 3]); // [1]
```

=> **drop(arr, n=1)**  
Creates a slice of array with n elements dropped from the beginning.

- arguments: arr(Array, n=1)
- returns: Array

Example:

```js
drop([1, 2, 3]); // [2, 3]
drop([1, 2, 3], 2); // [2,3]
drop([1, 2, 3], 5); // []
drop([1, 2, 3], 0); // [1, 2, 3]
```
