* https://www.codewars.com/kata/find-numbers-which-are-divisible-by-given-number/solutions/javascript
```javascript 
function divisibleBy(numbers, divisor) {
  var newArr = [];
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % divisor === 0) {
      newArr.push(numbers[i]);
    } 
  }
return newArr;
}

```
*https://www.codewars.com/kata/convert-a-string-to-an-array/train/javascript

```javascript
function stringToArray(string){
  return string.split(" ");
	}
```
*https://www.codewars.com/kata/determine-offspring-sex-based-on-genes-xx-and-xy-chromosomes/train/javascript

```javascript
function chromosomeCheck(sperm) {
  return sperm === 'XY' ? "Congratulations! You're going to have a son." :
  "Congratulations! You're going to have a daughter.";
}
```