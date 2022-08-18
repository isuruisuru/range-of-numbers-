# Use Recursion to Create a Range of Numbers in JavaScript

* This is the 113<sup>th</sup> activity in __freeCodeCamp__ Basic JavaScript course.

> We have defined a function named `rangeOfNumbers` with two parameters. The function should return __an array of integers__ which begins with a number represented by the `startNum` parameter and ends with a number represented by the `endNum` parameter. The starting number will always be __less than or equal to the ending number__. Your function __must use recursion__ by calling itself and not use loops of any kind. It should also work for cases where both `startNum` and `endNum` are the same.

### Please try to do this acctivity on your own first and only refer this to clear any doubts.
<hr>

## Code:
```javascript
function rangeOfNumbers(startNum, endNum) {
  return (startNum>endNum) ? [] : [startNum].concat(rangeOfNumbers(startNum+1,endNum)); 
};

console.log(rangeOfNumbers(-5, 5))
```

Output for the given parameters is:
__[ -5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5 ]__
