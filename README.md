# 🔢 Word Counter

A lightweight JavaScript utility for counting word occurrences in a sentence and printing individual characters from a string.

---

## 📁 Project Structure

```
word-counter/
├── README.md
└── main.js
```

---

## 🚀 Features

- **Character Printer** — Iterates over a string and logs each character individually.
- **Word Matcher** — Counts how many times a specific word appears in an array of words, with real-time logging of each comparison.

---

## 📄 Functions

### `printCharacters(str)`

Prints each character of a string on a new line.

| Parameter | Type | Description |
|---|---|---|
| `str` | `string` | The string to iterate over |

**Example:**
```js
printCharacters("hello");
// Output:
// h
// e
// l
// l
// o
```

---

### `getMatchedWordCount(sentence, match)`

Counts the number of times a word appears in an array of words. Logs each comparison step along the way.

| Parameter | Type | Description |
|---|---|---|
| `sentence` | `string[]` | Array of words to search through |
| `match` | `string` | The word to search for |

**Returns:** `number` — the total count of matched words.

**Example:**
```js
getMatchedWordCount(
  ["I", "really", "really", "really", "like", "to", "code"],
  "really"
);
// Checking "I" against "really" | Running count: 0
// Checking "really" against "really" | Running count: 1
// Checking "really" against "really" | Running count: 2
// Checking "really" against "really" | Running count: 3
// ...
// Returns: 3
```

---

## ▶️ Usage

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) installed.

### Run the script

```bash
node main.js
```

### Expected Output

```
h
e
l
l
o
Checking "I" against "really" | Running count: 0
Checking "really" against "really" | Running count: 1
Checking "really" against "really" | Running count: 2
Checking "really" against "really" | Running count: 3
Checking "like" against "really" | Running count: 3
Checking "to" against "really" | Running count: 3
Checking "code" against "really" | Running count: 3
3
Checking "Do" against "dandy" | Running count: 0
Checking "not" against "dandy" | Running count: 0
Checking "fear" against "dandy" | Running count: 0
Checking "the" against "dandy" | Running count: 0
Checking "dandy" against "dandy" | Running count: 1
Checking "lion" against "dandy" | Running count: 1
1
```

---

## 🛠️ Built With

- **JavaScript (ES6+)** — `for...of` loops, template literals
- **Node.js** — Runtime environment
