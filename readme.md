##Hello

---
6/25/2019
https://www.codewars.com/kata/find-numbers-which-are-divisible-by-given-number/solutions/javascript

function divisibleBy(numbers, divisor) {
  var newArr = [];
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % divisor === 0) {
      newArr.push(numbers[i]);
    } 
  }
return newArr;
}