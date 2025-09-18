# JavaScript Methods Reference Guide

Complete guide to the main JavaScript methods organized by category.

## String Methods

### Transformation
- `toUpperCase()` - Converts to uppercase
- `toLowerCase()` - Converts to lowercase
- `trim()` - Removes whitespace from both ends
- `trimStart()` - Removes whitespace from beginning
- `trimEnd()` - Removes whitespace from end
- `replace()` - Replaces first occurrence
- `replaceAll()` - Replaces all occurrences
- `repeat()` - Repeats string n times

### Search and Verification
- `indexOf()` - Index of first occurrence
- `lastIndexOf()` - Index of last occurrence
- `includes()` - Checks if contains substring
- `startsWith()` - Checks if starts with substring
- `endsWith()` - Checks if ends with substring
- `search()` - Search with regex
- `match()` - Find matches
- `matchAll()` - Find all matches

### Extraction
- `substring()` - Extracts part of string
- `substr()` - Extracts characters from index
- `slice()` - Extracts section of string
- `charAt()` - Returns character at index
- `charCodeAt()` - Returns Unicode code of character
- `split()` - Splits string into array

## Array Methods

### Transformation
- `map()` - Transforms each element
- `filter()` - Filters elements by condition
- `reduce()` - Reduces array to single value
- `reduceRight()` - Reduce from right to left
- `sort()` - Sorts elements
- `reverse()` - Reverses element order

### Addition/Removal
- `push()` - Adds element(s) at end
- `pop()` - Removes last element
- `unshift()` - Adds element(s) at beginning
- `shift()` - Removes first element
- `splice()` - Adds/removes elements at specific position
- `slice()` - Extracts section of array

### Search
- `find()` - Finds first element matching condition
- `findIndex()` - Index of first element matching condition
- `findLast()` - Finds last element matching condition
- `indexOf()` - Index of first occurrence
- `lastIndexOf()` - Index of last occurrence
- `includes()` - Checks if array contains element

### Iteration
- `forEach()` - Executes function for each element
- `some()` - Tests if any element matches condition
- `every()` - Tests if all elements match condition
- `entries()` - Returns iterator of [index, value]
- `keys()` - Returns iterator of indices
- `values()` - Returns iterator of values

### Others
- `join()` - Joins elements into string
- `concat()` - Concatenates arrays
- `flat()` - Flattens nested arrays
- `flatMap()` - Map + flat in one operation

## Object Methods

- `Object.keys()` - Returns array of keys
- `Object.values()` - Returns array of values
- `Object.entries()` - Returns array of [key, value] pairs
- `Object.assign()` - Copies properties between objects
- `Object.create()` - Creates object with specific prototype
- `Object.freeze()` - Makes object immutable
- `Object.seal()` - Prevents addition/removal of properties
- `Object.hasOwnProperty()` - Checks if has own property
- `Object.defineProperty()` - Defines property with descriptors
- `Object.getOwnPropertyNames()` - Names of own properties

## Number Methods

### Conversion
- `toString()` - Converts to string
- `toFixed()` - Fixes decimal places
- `toPrecision()` - Sets precision
- `parseInt()` - Parses string to integer
- `parseFloat()` - Parses string to float

### Validation
- `isNaN()` - Checks if is NaN
- `isFinite()` - Checks if is finite number
- `Number.isInteger()` - Checks if is integer
- `Number.isSafeInteger()` - Checks if is safe integer

## Date Methods

### Get/Set Date Components
- `getDate()` / `setDate()` - Day of month
- `getMonth()` / `setMonth()` - Month (0-11)
- `getFullYear()` / `setFullYear()` - Full year
- `getDay()` - Day of week (0-6)
- `getHours()` / `setHours()` - Hours
- `getMinutes()` / `setMinutes()` - Minutes
- `getSeconds()` / `setSeconds()` - Seconds
- `getTime()` / `setTime()` - Timestamp

### Formatting
- `toString()` - String representation
- `toDateString()` - Date portion as string
- `toTimeString()` - Time portion as string
- `toISOString()` - ISO format string
- `toLocaleDateString()` - Locale date string
- `toLocaleTimeString()` - Locale time string

## Math Methods

### Rounding
- `Math.round()` - Rounds to nearest integer
- `Math.floor()` - Rounds down to integer
- `Math.ceil()` - Rounds up to integer
- `Math.trunc()` - Removes decimal part

### Min/Max/Random
- `Math.max()` - Returns largest value
- `Math.min()` - Returns smallest value
- `Math.random()` - Random number between 0-1

### Power/Root
- `Math.pow()` - Power calculation
- `Math.sqrt()` - Square root
- `Math.cbrt()` - Cube root

### Other
- `Math.abs()` - Absolute value
- `Math.sign()` - Sign of number
- `Math.PI` - Pi constant
- `Math.E` - Euler's constant

## Promise Methods

### Instance Methods
- `then()` - Handles fulfilled promise
- `catch()` - Handles rejected promise
- `finally()` - Always executes

### Static Methods
- `Promise.all()` - Waits for all promises
- `Promise.allSettled()` - Waits for all to settle
- `Promise.race()` - First promise to settle
- `Promise.any()` - First promise to fulfill
- `Promise.resolve()` - Creates resolved promise
- `Promise.reject()` - Creates rejected promise

## JSON Methods

- `JSON.stringify()` - Converts object to JSON string
- `JSON.parse()` - Parses JSON string to object

## Console Methods

### Logging
- `console.log()` - Standard output
- `console.error()` - Error output
- `console.warn()` - Warning output
- `console.info()` - Information output
- `console.debug()` - Debug output

### Formatting
- `console.table()` - Displays data as table
- `console.group()` / `console.groupEnd()` - Groups messages
- `console.groupCollapsed()` - Collapsed group

### Performance
- `console.time()` / `console.timeEnd()` - Measures execution time
- `console.count()` - Counts function calls
- `console.trace()` - Stack trace

## DOM Methods (Browser)

### Selection
- `document.getElementById()` - Select by ID
- `document.getElementsByClassName()` - Select by class
- `document.getElementsByTagName()` - Select by tag
- `document.querySelector()` - Select first match (CSS selector)
- `document.querySelectorAll()` - Select all matches (CSS selector)

### Element Methods
- `element.appendChild()` - Add child element
- `element.removeChild()` - Remove child element
- `element.insertBefore()` - Insert before element
- `element.cloneNode()` - Clone element
- `element.getAttribute()` / `element.setAttribute()` - Get/set attributes
- `element.classList.add()` / `element.classList.remove()` - Modify classes
- `element.addEventListener()` - Add event listener

### Content
- `element.innerHTML` - HTML content
- `element.textContent` - Text content
- `element.style` - CSS styles

## Error Handling

- `try...catch...finally` - Error handling block
- `throw` - Throws custom error
- `Error()` - Creates error object
- `TypeError()` - Type error
- `ReferenceError()` - Reference error