# Methods

<h1>map()</h1>
<h3>Description of method:</h3>
- Creates a new array with the results of calling a function for every array element. It calls the provided function once for each element in an array, in order.
<h3>How it works:</h3>
- A provided function is called on every element in the array that it's being called on. There is then a new array populated with the results from calling the function.
<h3>Syntax:</h3>

```
array.map(function(currentValue, index, arr), thisValue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
const nums = [10, 40, 62]
const newNums = nums.map(theFunc)

function theFunc(num) {
  return num + 100;
}
```

<h3>Example:</h3>

```js
const location = [
  { trip: 'Mexico', price: 250 },
  { trip: 'Jordan', price: 875 },
  { trip: 'Japan', price: 900 },
  { trip: 'Denmark', price: 700 }
 ]

const locationName = location.map((item) => {
  return location.trip
  return location.price
 })
 ```

<h3>Example:</h3>

```js
const numbers = [4, 2, 7, 10]
const newArr = numbers.map(function(num) {
  return num * 5
})
```

<h1>reduce()</h1>
<h3>Description of method:</h3>
- Reduces the array to a single value. It executes a provided function for each value of an array from left to right. The returned value of the function is stored in an accumulator.
<h3>How it works:</h3>
- Provide a reducer function that will be executed on each element of an array to produce a single output value.
<h3>Syntax:</h3>

```
array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
const arr = [4, 9, 15, 22]
const reducer = (accumulator, currentVal) {
  return accumulator + currentVal
}, 1)
 ```

<h3>Example:</h3>

```js
const dollars = [2.5, 10.25, .75];
const sum = dollars.reduce( function(total, amount){
  return total + amount
});

sum //13.5
```

<h3>Example:</h3>

```js
let val = 8
let sum = [{x: 4}, {x: 7}, {x: 1}].reduce(
  (accumulator, currentVal) => accumulator + currentVal.x
  , val)
```

<h1>filter()</h1>
<h3>Description of method:</h3>
- Creates an array filled with all array elements that pass a test provided as a function.
<h3>How it works:</h3>
- Creates a new array with all elements that pass the test implemented by the provided function.
<h3>Syntax:</h3>

```
array.filter(function(currentValue, index, arr), thisValue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
const ages = [18, 25, 15, 33];

function isAdult(age) {
  return age >= 18;
 }
```
 
<h3>Example:</h3>

```js
let books = [
  {name: 'Catcher in the rye', pages: 277},
  {name: 'The House of Spirits', pages: 496},
  {name: 'To Kill a Mockingbird', pages: 281},
  {name: 'The Universe and the Teacup', pages: 227}
  
  let bigBooks = books.filter(page) {
    return page >= 250;
 }
```

<h3>Example:</h3>

```js
function positiveNum(value) {
  return value > 0;
}

var filtered = [0, 333, 80, 152, 5].filter(posNum);
print(filtered);
```

<h1>forEach()</h1>
<h3>Description of method:</h3>
- Executes a provided function once for each array element. 
<h3>How it works:</h3>
- Takes the provided function and calls it once for each element in order.
<h3>Syntax:</h3>

```
array.forEach(function(currentValue, index, arr), thisValue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
let colors = ["black", "yellow", "red", "green", "aqua"];

function colorsAndIndex (item, index){
console.log(`${item} has index ${index}`);
}
colors.forEach(colorsAndIndex);

```

<h3>Example:</h3>

```js
function sum() {
  let items = [15, 33, 50];
  let copy = [];

  itms.forEach(function (item) {
    copy.push(item + item+5);
  });
 
 document.write(copy);
}
 sum();
```

<h3>Example:</h3>

```js
const items = [15, 33, 50];
let copy = [];

items.forEach(function(item){
  copy.push(item*item);
});
print(copy);
```

<h1>sort()</h1>
<h3>Description of method:</h3>
- Sorts items of an array either alphabetically or numerically, and either ascending or descending. 
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.sort(compareFunction)
```

<h3>Time Complexity:</h3>
O(nlog(n))
<h3>Example:</h3>

```js
let famMembers = ['Jane', 'Cesar', 'Ulises', 'Maria', 'Ella'];
famMembers.sort();
```

<h3>Example:</h3>

```js
let nums = [5, 21, 36, 9];
nums.sort();
```

<h3>Example:</h3>

```js
let nums = [5, 21, 36, 9];
nums.sort(function(a, b){return a-b});
```

<h1>slice()</h1>
<h3>Description of method:</h3>
- Extracts a section of a string and retuns it as a new string, without modifiying the original string.
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.slice(start, end)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
let colors = ['black', 'blue', 'teal', 'coral', 'red'];

colors.slice(0,2);

```
<h3>Example:</h3>
<h3>Example:</h3>

<h1>pop()</h1>
<h3>Description of method:</h3>
- Removes the last element of an array, and returns that element.
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.pop()
```

<h3>Time Complexity:</h3>
O(1)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>shift()</h1>
<h3>Description of method:</h3>
- Removes the first item of an array.
<h3>How it works:</h3>

<h3>Syntax:</h3>
```
array.shift()
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>push()</h1>
<h3>Description of method:</h3>
- Adds new items to the end of an array, and returns the new length.
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.push(item1, item2, ..., itemX)
```

<h3>Time Complexity:</h3>
O(1)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>unshift()</h1>
<h3>Description of method:</h3>
- Adds new items to the beginning of an array, and returns the new length. 
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.unshift(tem1, item2, ..., itemX)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>includes()</h1>
<h3>Description of method:</h3>
- Determines whether a string contains the characters of a specified string. The method returns true if the string contains the characters and, false if not.
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
string.includes(searchvalue, start)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>indexOf()</h1>
<h3>Description of method:</h3>
- Searches the array for the specified item and returns its position. The search will start at the specified position or at the beginning if no start position is specified. (Returns -1 if the item is not found.
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.indexOf(item, start)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>every()</h1>
<h3>Description of method:</h3>
- Tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value)
<h3>How it works:</h3>

<h3>Syntax:</h3>

```
array.every(function(currentValue, index, arr), thisValue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>charAt()</h1>
<h3>Description of method:</h3>
- Returns the character at the specified index in a sting.
<h3>How it works:</h3>
It outputs a character depending on the index of the value. The index of the first character is 0, the next is 1, then 2, and so on. 
<h3>Syntax:</h3>

```
public char charAt(int index)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>charCodeAt()</h1>
<h3>Description of method:</h3>
- Returns the Unicode of the character at the specified index in a string.
<h3>How it works:</h3>
You specify an index and the method returns an integer between 0 and 65535 representing the UTF- 16 code unit at the given index.
<h3>Syntax:</h3>

```
string.charCodeAt(index)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>concat()</h1>
<h3>Description of method:</h3>
- Used to join two or more strings. It does not change the existing strings, instead, it returns a new string containing the text of the joined strings.
<h3>How it works:</h3>
If you have multiple strings and want to join them yet not change them then you can concatenate them by using the concat method.
<h3>Syntax:</h3>

```
string.concat(string1, string2, ..., stringX)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>includes()</h1>
<h3>Description of method:</h3>
- Determines whether an array includes a certain value among its entries, returning true or false as appropriate.
<h3>How it works:</h3>
Look for a value within an array. If the value is withing the array it will return true, if not, will return false.

<h3>Syntax:</h3>

```
includes(searchElement)
includes(searchElement, fromIndex)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>indexOf()</h1>
<h3>Description of method:</h3>
- Returns the first index at which a given element can be found in the array, or -1 if it is not present.
<h3>How it works:</h3>
The method will return the position of the first occurrence of a specified value in a string. If the value cannot be found then the return will be -1.
<h3>Syntax:</h3>

```
string.indexOf(searchvalue, start)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>

```js
```
<h3>Example:</h3>
<h3>Example:</h3>


<h1>match()</h1>
<h3>Description of method:</h3>
- Searches a string for a match against a regular expression, and returns the matches, as an Array object.
<h3>How it works:</h3>
The method retrieves the result by matching a string against the regular expression to return a new array.
<h3>Syntax:</h3>

```
string.match(regexp)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

<h1>repeat()</h1>
<h3>Description of method:</h3>
- Constructs and returns a new sting which contains the specified number of copies of the string on which it was called, concatenated together.
<h3>How it works:</h3>
The method returns a new string with a specified number of copies of the string it was called on.
<h3>Syntax:</h3>

```
string.repeat(count)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>replace()</h1>
<h3>Description of method:</h3>
- Returns a new string with some or all matches of a pattern replaced by a string or a function to be called for each match. (If a pattern is a string, only the first occurrence will be replaced.
<h3>How it works:</h3>
Replaces a specified phrase with another specified phrase.
<h3>Syntax:</h3>

```
string.replace(oldvalue, newvalue, count)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>search()</h1>
<h3>Description of method:</h3>
- Searches a string or a regular expression for a specified value, and returns the position of the match or -1 if a match is not found.
<h3>How it works:</h3>
The method executes a search for a match between a regular expression and the string object.
<h3>Syntax:</h3>

```
string.search(searchvalue)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>splice()</h1>
<h3>Description of method:</h3>
- Adds/removes items to/from an array, and returns the removed item(s).
<h3>How it works:</h3>
The method changes the contents of an array by removing or replacing the existing elements and/or adding new elements in it's place.
<h3>Syntax:</h3>

```
array.splice(index, howmany, item1, ....., itemX)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>split()</h1>
<h3>Description of method:</h3>
- Splits a string into an array of substrings, and returns the new array.
<h3>How it works:</h3>
The method divides a string in an ordered list of substrings and puts them into an array. The division is done by searching for a pattern.
<h3>Syntax:</h3>

```
string.split(separator, limit)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>substr()</h1>
<h3>Description of method:</h3>
- Returns a portion of the string, starting at the specified index and extending for a given number of characters afterwards.
<h3>How it works:</h3>
The method extracts part of a string, beginning at the character of the specified position, and returns the specified number of characters.
<h3>Syntax:</h3>

```
string.substr(start, length)
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>toLowerCase()</h1>
<h3>Description of method:</h3>
- Converts a string to lowercase letters
<h3>How it works:</h3>
Returns the calling string value converted to lowercase
<h3>Syntax:</h3>

```
string.toLowerCase()
```

<h3>Time Complexity:</h3>

<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>toUpperCase()</h1>
<h3>Description of method:</h3>
- Converts a string to uppercase letters.
<h3>How it works:</h3>
The method returns the calling string value converted to uppercase.
<h3>Syntax:</h3>

```
string.toUpperCase()
```

<h3>Time Complexity:</h3>
O(n)
<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>


<h1>trim()</h1>
<h3>Description of method:</h3>
- Removes whitespace from both sides of a string.
<h3>How it works:</h3>
The method removes white space from the ends including all the whitespace characters such as space, tab, no-break space, etc.
<h3>Syntax:</h3>

```
string.trim()
```

<h3>Time Complexity:</h3>

<h3>Example:</h3>
<h3>Example:</h3>
<h3>Example:</h3>

