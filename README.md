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
* https://www.codewars.com/kata/convert-a-string-to-an-array/train/javascript

```javascript
function stringToArray(string){
  return string.split(" ");
	}
```
* https://www.codewars.com/kata/determine-offspring-sex-based-on-genes-xx-and-xy-chromosomes/train/javascript

```javascript
function chromosomeCheck(sperm) {
  return sperm === 'XY' ? "Congratulations! You're going to have a son." :
  "Congratulations! You're going to have a daughter.";
}
```
* https://www.codewars.com/kata/thinkful-logic-drills-traffic-light/train/javascript

```javascript
function updateLight(current) {
 if (current === "green"){
   return "yellow";
   } else if (current === "yellow"){
   return "red"}
   else if(current === "red"){
   return "green"}
   }
   ```
   * https://www.codewars.com/kata/palindrome-strings/train/javascript
   
   ```javascript
   
   function isPalindrome(line) {
     
     let half1 = '';
     
      for (let i = line.length -1; i >= 0; i --){
       half1 += line[i];
     }
     return half1 === line ? true : false;
   
   ```
   * https://www.codewars.com/kata/get-list-sum-recursively/train/javascript
   
  ```javascript 
  
  function sumR(x) {
    
    if ( x.length === 0 ){
      
    return 0;
    } else {
      return x.shift() + sumR(x);
    }
  }
  
  ```
  
 * https://www.codewars.com/kata/the-feast-of-many-beasts/train/javascript
 
 ```javascript 
 
 function feast(beast, dish) {
   if (beast[0] == dish[0] && beast[beast.length - 1] == dish[dish.length - 1]) {
     return true;
   }
   else {return false;}
 }
 
 ```
 * https://www.codewars.com/kata/simple-multiplication/train/javascript
 
 ```javascript
  
  function simpleMultiplication(number) {
    return number % 2 === 0  ? number * 8 : number * 9; 
  }
  
  ```
  
  * https://www.codewars.com/kata/type-of-sum/train/javascript
  
  ```javascript
  
  function typeOfSum(a, b) {
    return typeof (a + b);
  }
  
  ``` 
  * https://www.codewars.com/kata/sleigh-authentication/train/javascript
  
   ```javascript
   
   function Sleigh() {}
   
   Sleigh.prototype.authenticate = function(name, password) {
     return name === "Santa Claus" && password === "Ho Ho Ho!"?
     true : false;
   }
   
   ```
   * https://www.codewars.com/kata/convert-a-string-to-a-number/train/javascript
   
   ```javascript
   
   var stringToNumber = function(str){
     return Number(str);
   }
   
   ```
  * https://www.codewars.com/kata/56f6ad906b88de513f000d96
 
 ```javascript 
 function bonusTime(salary, bonus) {
 return bonus === true ? '£' + (salary * 10) : '£' + salary;
 }
 
 ``` 
 * Holiday VI - Shark Pontoon
  
  ```javascript
   
 function shark(pontoonDistance, sharkDistance, youSpeed, sharkSpeed, dolphin){
 if(dolphin){
     sharkSpeed /= 2;
   }
   return pontoonDistance/youSpeed < sharkDistance/sharkSpeed ? "Alive!" : "Shark Bait!";
 }
 
 
 ``` 
 * https://www.codewars.com/kata/alphabet-symmetry/train/javascript
 
 ```javascript 
 
 function solve(arr){  
   let alp = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
   let arrN = [];
     for(let i = 0; i < arr.length; i++){
       let count = 0;
         for(let j = 0; j < arr[i].length; j++){
           if( j === alp.indexOf(arr[i][j].toUpperCase()) ){
             count++;
           }
         }
         arrN.push(count);
     }
   return arrN;
 };
```
* https://www.codewars.com/kata/arrays-similar/train/javascript

```javascript

function arraysSimilar(arr1, arr2) {
  if(arr1.length !== arr2.length) return false;
    arr1.sort();
    arr2.sort();
  for(let i = 0; i < arr1.length; i++) {
    if(arr1[i] !== arr2[i]) return false; 
  }
  return true;
}
```


* https://www.codewars.com/kata/spongebob-meme/train/javascript

```javascript

function spongeMeme(sentence) {
  let res = '';
    for(let i = 0; i < sentence.length; i++) {
      res += (i % 2) ? sentence[i].toLowerCase() : sentence[i].toUpperCase();
    }
  return res;
}

```
* https://www.codewars.com/kata/valid-parentheses/train/javascript

```javascript

function validParentheses(parens) {
  let arr = parens.split('');
  let cnt = 0;
  
  for (let i = 0; i < parens.length; i++) {
    if (arr[i] === '(') cnt++;
    else if (arr[i] === ')') cnt--;
    if (cnt < 0) return false;
  }
  if (cnt === 0) return true;
  else return false;
}

```
* https://www.codewars.com/kata/5302d846be2a9189af0001e4/solutions/javascript

```javascript

const sayHello = ( name, city, state ) => `Hello, ${name.join(' ')}! Welcome to ${city}, ${state}!`;

```

* https://www.codewars.com/kata/sort-the-odd/train/javascript

```javascript

function sortArray(array) {
  let odd = array.filter(a => a % 2 !== 0).sort((a,b) => a - b);
  let res = array.map(a => a % 2 !== 0 ? odd.shift() : a);
  return res;
}

```