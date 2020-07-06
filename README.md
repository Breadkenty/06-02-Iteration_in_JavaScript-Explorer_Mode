# 06-02 Iteration in JavaScript Explorer Mode

### My solution:

```javascript
/**
 * 1) Define a function named `yelling` that takes an array of
 * strings as an argument and returns a new array with all
 * the words forced to uppercase
 *
 * Example:
 *
 * const yelling = (array) => {
 *    // your code here
 * }
 */

// ...
const yelling = array => {
  return array.map(word => word.toUpperCase())
}

/**
 *
 * 2) Define a function named `doubleTrouble` that takes an array of
 * numbers as an argument and returns a new array with all
 * the numbers multiplied by 2
 */

// ...
const doubleTrouble = array => {
  return array.map(number => number * 2)
}

/*
 * 3) Define a function stringyIndexes() that takes an array of
 * strings as an argument and returns a new array with each string
 * suffixed with " is at index X" where X is the index of the element
 */

// ...
const stringyIndexes = array => {
  return array.map((word, index) => `${word} is at index ${index}`)
}

/*
 * 4) Define a function onlyTheEvenSurvive that accepts an array of
 * numbers and returns only the elements that are even
 */

// ...
const onlyTheEvenSurvive = array => {
  return array.filter(number => number % 2 === 0)
}

/*
 * 5) Define a function onlyTheEvenIndexedSurvive that accepts an array of
 * numbers and returns only the elements at indexes that are even
 */

// ...
const onlyTheEvenIndexedSurvive = array => {
  return array.filter((number, index) => index % 2 === 0)
}

/*
 * 6)  Define a function bestMoviesOfTheYear that accepts an array of
 * movie objects AND a year and returns the names of movies that are
 * from that year AND have a score more than 90
 *
 * A movie object looks like this:
 *
 * {
 *   name: "Get Out",
 *   year: "2017",
 *   score: 99
 * }
 */

// ...
const bestMoviesOfTheYear = (array, year) => {
  return array
    .filter(movie => movie.score > 90 && movie.year === year)
    .map(movie => movie.name)
}

/*
 * 7) Define a function everyoneIsOdd that accepts an array of
 * numbers and returns true if every element of the array is
 * odd.
 */

// ...
const everyoneIsOdd = array => {
  return array.every(number => number % 2 === 1)
}

/*
 * 8) Define a function findTheNeedle that accepts an array of
 * strings and returns the one string that contains the word
 * `needle` inside
 */

// ...
const findTheNeedle = array => {
  return array.find(string => string.includes('needle'))
}

/*
 * 9) Define a function findTheNeedleIndex that accepts an array of
 * strings and returns the index of the string that contains
 *  the word `needle` inside
 */

// ...
const findTheNeedleIndex = array => {
  return array.findIndex(string => string.includes('needle'))
}

/*
 *` 10)  Define a function someoneToLove that accepts an array of
 * strings and returns true if at least one string is exactly
 * four characters long
 */

// ...
const someoneToLove = array => {
  return array.some(string => string.length === 4)
}

/*
 * 11) Define a function mapYourself that accepts an array of
 * numbers and returns a new array where each number is doubled.
 *
 * However, you cannot use any of the Array enumerables.
 *
 * So no using forEach, map, filter, reduce, etc.
 */

// ...
const mapYourself = array => {
  let newArray = []
  for (var index = 0; index < array.length; index++) {
    newArray.push(array[index] * 2)
  }
  return newArray
}

/*
 * 12) Define a function filterYourself that accepts an
 * array of numbers and returns a new array containing
 * only the even numbers.
 *
 * However, you cannot use any of the Array enumerables.
 *
 * So no using forEach, map, filter, reduce, etc.
 */

// ...
const filterYourself = array => {
  let newArray = []
  for (var index = 0; index < array.length; index++) {
    if (array[index] % 2 === 0) {
      newArray.push(array[index])
    }
  }
  return newArray
}

/*
 * 13) Define a function everyYourself that accepts an
 * array of numbers and returns true if every number
 * in the array is even.
 *
 * However, you cannot use any of the Array enumerables.
 *
 * So no using forEach, map, filter, reduce, etc.
 */

// ...

const everyYourself = array => {
  let everyNumberIsEven = true
  for (var index = 0; index < array.length; index++) {
    if (array[index] % 2 === 1) {
      everyNumberIsEven = false
    }
  }
  return everyNumberIsEven
}
```

# Assignment Overview:

## Objectives

After completing this assignment, you should be able to:

- Demonstrate understanding of iteration/enumeration

## Instructions

1. Fork [this repository](https://github.com/suncoast-devs/js-iteration) to your own account.
2. Change into your projects directory:
3. Clone your repository: `hub clone js-iteration`
4. Change into your project's directory: `cd js-iteration`
5. Install the dependencies: `yarn install` (or just `yarn` for short)
6. Open in your editor]
7. Start the test runner: `yarn test`
8. Open `src/functions.test.js` and work on functions until tests pass.
9. Commit and push your work to GitHub.
10. Turn in the URL to your GitHub repo.

## Explorer Mode

- All tests passing

## Additional Resources

Reference the documentation on DevDocs to find what kind of helpful functions
might already be in JavaScript.

- [String Functions on DevDocs](https://devdocs.io/javascript/global_objects/string).
- [Array Functions on DevDocs](http://devdocs.io/javascript/global_objects/array).
