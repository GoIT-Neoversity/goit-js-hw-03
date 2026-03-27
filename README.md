# JavaScript Arrays

This project contains solutions focused on functions and arrays.

---

## Project Structure

```
├── js/
│ ├── task-1.js
│ ├── task-2.js
│ └── task-3.js
│ └── task-3.js
├── index.html
├── .gitignore
├── .prettierrc
└── README.md
```

---

## Tasks

### Task 1 — Slug generator

File: [js/task-1.js](./js/task-1.js)

Function `slugify(title)` converts an article title into a URL-friendly slug: lowercase words joined by hyphens.

**Parameters**

| Parameter | Type   | Description          |
| --------- | ------ | -------------------- |
| `title`   | string | Article title string |

**Returns** `string` — slug built from the title.

**Examples**

```js
slugify('Arrays for begginers'); // "arrays-for-begginers"
slugify('English for developer'); // "english-for-developer"
slugify('Ten secrets of JavaScript'); // "ten-secrets-of-javascript"
slugify('How to become a JUNIOR developer in TWO WEEKS'); // "how-to-become-a-junior-developer-in-two-weeks"
```

---

### Task 2 — Combine arrays

File: [js/task-2.js](./js/task-2.js)

Function `makeArray(firstArray, secondArray, maxLength)` combines two arrays and trims the result to `maxLength` elements if needed.

**Parameters**

| Parameter     | Type   | Description                              |
| ------------- | ------ | ---------------------------------------- |
| `firstArray`  | Array  | First source array                       |
| `secondArray` | Array  | Second source array                      |
| `maxLength`   | number | Maximum number of elements in the result |

**Returns** `Array` — combined (and possibly trimmed) array.

**Examples**

```js
makeArray(['Mango', 'Poly'], ['Ajax', 'Chelsea'], 3); // ["Mango", "Poly", "Ajax"]
makeArray(['Mango', 'Poly', 'Houston'], ['Ajax', 'Chelsea'], 4); // ["Mango", "Poly", "Houston", "Ajax"]
makeArray(['Mango'], ['Ajax', 'Chelsea', 'Poly', 'Houston'], 3); // ["Mango", "Ajax", "Chelsea"]
makeArray(['Earth', 'Jupiter'], ['Neptune', 'Uranus'], 2); // ["Earth", "Jupiter"]
makeArray(['Earth', 'Jupiter'], ['Neptune', 'Uranus'], 4); // ["Earth", "Jupiter", "Neptune", "Uranus"]
makeArray(['Earth', 'Jupiter'], ['Neptune', 'Uranus', 'Venus'], 0); // []
```

---

### Task 3 — Filter numbers array

File: [js/task-3.js](./js/task-3.js)

Function `filterArray(numbers, value)` returns a new array containing only the numbers that are greater than `value`.

**Parameters**

| Parameter | Type   | Description                    |
| --------- | ------ | ------------------------------ |
| `numbers` | Array  | Array of numbers to filter     |
| `value`   | number | Threshold — keep numbers above |

**Returns** `Array` — filtered array of numbers greater than `value`.

**Examples**

```js
filterArray([1, 2, 3, 4, 5], 3); // [4, 5]
filterArray([1, 2, 3, 4, 5], 4); // [5]
filterArray([1, 2, 3, 4, 5], 5); // []
filterArray([12, 24, 8, 41, 76], 38); // [41, 76]
filterArray([12, 24, 8, 41, 76], 20); // [24, 41, 76]
```
