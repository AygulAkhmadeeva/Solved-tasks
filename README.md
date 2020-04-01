# Solved-tasks
* task 1
```javascript
//://www.codewars.com/kata/is-he-gonna-survive/train/javascript
//Is he gonna survive?
function hero(bullets, dragons){
return dragons*2 <= bullets ;
}
```
* task 2
```javascript
//https://www.codewars.com/kata/breaking-chocolate-problem/train/javascript
//Breaking chocolate problem
function breakChocolate(n,m) {
console.log(n,m);
if (n>0 && m>0) {
  if (n>m) {
    return (n-1)*m + m-1;
    } else {
    return (m-1)*n + n-1;
    }
  }
      return 0;
}
```
* task 3
```javascript
// https://www.codewars.com/kata/well-of-ideas-easy-version/train/javascript
// Well of Ideas - Easy Version
function well(x){
console.log(x);
 let j = 0;
  for (let i=0; i<x.length; i++) {
   if (x[i] === 'good') j+=1;
   }
 if (j===1 || j===2) return 'Publish!';
 if (j>2) return 'I smell a series!';
 if (j<1) return 'Fail!';
}
```
* task 4
```javascript
//https://www.codewars.com/kata/merge-two-sorted-arrays-into-one/train/javascript
//Merge two sorted arrays into one
function mergeArrays(arr1, arr2) {
console.log(arr1, arr2);
  let newArr = [];
   for(let i=0; i<arr1.length; i++) {
    arr2.push(arr1[i]);
    }
  newArr = arr2.sort((a,b) => a-b);
  let uniqArr = Array.from(new Set(newArr));
  return uniqArr;
}
```

```javascript
//https://www.codewars.com/kata/return-the-closest-number-multiple-of-10/train/javascript
//Return the closest number multiple of 10
const closestMultiple10 = num => {
console.log(num);
 if (num%10 < 5) return num - (num %10);
 if (num%10 >= 5) return num + 10 - num % 10;
};
```

```javascript
//Area of a Square
//https://www.codewars.com/kata/area-of-a-square/train/javascript
function squareArea(A){
console.log(A);
const cu = 4*A*A/(Math.PI*Math.PI)
return +cu.toFixed(2);
  }
```
//Calculate Two People's Individual Ages #7
https://www.codewars.com/kata/calculate-two-peoples-individual-ages/train/javascript
function getAges(s,d){
console.log(s,d);
if (s<0 || d<0 || d>s) return null;
const arr = [];
arr[1] = (s-d)/2;
arr[0] = arr[1]+d;
return arr;
};
```javascript
//https://www.codewars.com/kata/is-this-a-triangle/train/javascript
//Is this a triangle? #7
function isTriangle(a,b,c) {
 return (a + b > c && a + c > b && b + c > a);
 }
```

```javascript
//https://www.codewars.com/kata/power-of-two/train/javascript
//Power of two
let isPowerOfTwo = (n) => !(n & (n - 1)) && n != 0;
```

```javascript
//https://www.codewars.com/kata/factorial-1/train/javascript
//7 kyu Factorial
function factorial(n){
if (n === 0) return 1;
return n*factorial(n-1);
}
```

```javascript
//https://www.codewars.com/kata/filter-the-number/train/javascript
//Filter the number #7
var FilterString = function(value) {
  //Complete this function :)
}
var FilterString = function(value) {
console.log(value);
  let mV = value.split('');
  let res = mV.filter((j) => j >= 0); //massiv s chislami
  return +res.join('');
  }     ORRRRRRRRRRR
const FilterString = value => {
  return Number(
    value
      .split("")
      .filter(ele => Number(ele) == ele)
      .join("")
  );
};

 //&& isNaN(value[i])

```

```javascript
//Square Every Digit #7
//https://www.codewars.com/kata/square-every-digit/train/javascript
function squareDigits(num){
console.log(num);
let newArr =[];
  array = num.toString().split("");
for (let i=0; i< array.length; i++){
newArr.push(array[i]*array[i]);
  }
  return +newArr.join('');
   }

```

```javascript
//https://www.codewars.com/kata/enumerable-magic-number-1-true-for-all/train/javascript
//Enumerable Magic #1 - True for All?
function all( arr, fun ) {
  for(let i = 0; i < arr.length; i++) {
    if(!fun(arr[i])) {
      return false;
    }
  }
  return true;
}
```

```javascript
//https://www.codewars.com/kata/find-the-next-perfect-square/train/javascript
//Find the next perfect square!   7rank
const findNextSquare = (sq) => (Math.sqrt(sq) % 1 === 0) ?((Math.sqrt(sq)+1)*(Math.sqrt(sq)+1)) : -1;
```
```javascript
// https://www.codewars.com/kata/57efcb78e77282f4790003d8/solutions/javascript
//How many times should I go? #7
function howManyTimes(annualPrice, individualPrice) {
  return Math.ceil(annualPrice / individualPrice);
}
```

```javascript
//https://www.codewars.com/kata/every-possible-sum-of-two-digits/train/javascript
//Every possible sum of two digits #7
function digits(num){
const result = [];
    const parts = String(num).split('').map(n => n | 0);
    for(let i = 0; i < parts.length; i++) {
        for (let j = i + 1; j < parts.length; j++) {
            result.push(parts[i] + parts[j]);
        }
    }
    return result;
}
```

```javascript
//https://www.codewars.com/kata/formatting-decimal-places-number-1/train/javascript
//Formatting decimal places #1
function twoDecimalPlaces(number) {
return Math.trunc(number*100)/100;
}
```

```javascript
//https://www.codewars.com/kata/tortoise-racing/train/javascript
//Tortoise racing, rank #6
function race(v1, v2, g) {
   let arr = [];
   let t2 = g/(v2-v1); // time in h
   console.log(t2);
   if (t2<=0) return null;
   arr[0] = Math.trunc(t2); //h            
   arr[1] = Math.trunc((t2*60)%60); //min       
   arr[2] = Math.trunc((t2*3600)%60); //sec
   return arr;
}
```

```javascript
//https://www.codewars.com/kata/binary-addition/train/javascript
//Binary Addition
const addBinary = (a,b) => (a+b).toString(2);
```

```javascript
//https://www.codewars.com/kata/hex-to-decimal/train/javascript
//Hex to Decimal
function hexToDec(hexString){
return parseInt(hexString, 16);
}
```

```javascript
//Is every value in the array an array?
//https://www.codewars.com/kata/582c81d982a0a65424000201/train/javascript
const arrCheck = value => {
for (let i = 0; i < value.length; i++){
if ( Array.isArray(value[i])  ) continue;
else return false;
}
return true;
}
```

```javascript
//Find the first non-consecutive number
//https://www.codewars.com/kata/58f8a3a27a5c28d92e000144/train/javascript
function firstNonConsecutive (arr) {
console.log(arr);               
for (let i = 0; i < arr.length-1;i++){ 
    if ( arr[i+1] - arr[i] !== 1 ){                    
    return arr[i+1];                         
    }
  }  return null;
}

```

```javascript
//Enumerable Magic #3 - Does My List Include This?
//https://www.codewars.com/kata/545991b4cbae2a5fda000158/solutions/javascript
const include = (arr, item) => arr.includes(item);
```

```javascript
//Odd or Even?
function oddOrEven(arr) {
console.log(arr);
let sum = 0;                           
for (let i = 0; i < arr.length; i++){  
  sum += arr[i];                  
}
console.log(sum);
if (sum %2 === 0) {
return 'even';
} else {
return 'odd';
}
}
```

```javascript
//Remove the minimum
function removeSmallest(n) {
  let arr = [];
  let low = n[0];
  let lowInd = 0;
  for (let i = 1; i < n.length; i++){
     if (n[i]<low) {
     low = n[i];
     lowInd = i;
     }
  }
  return n.slice(0,lowInd).concat(n.slice(lowInd+1));  
}
```

```javascript
//Find the divisors! Cata7
// www.codewars.com/kata/544aed4c4a30184e960010f4/train/javascript
function divisors(integer) {
console.log(integer);
  let arr = [];
  for (let i=2; i<=integer; i++)
     {
     while (i<integer){
      if(integer % i === 0)
        {
        arr.push(i);
        }
        i++;
      }   
  }
  if (arr.length === 0) return integer + ' is prime';
  return arr;
  console.log(arr);
};
```

```javascript
//Training JS #4: Basic data types--Array
//https://www.codewars.com/kata/571effabb625ed9b0600107a/train/javascript
function getLength(arr){
  return arr.length;
}
function getFirst(arr){
   return arr[0];
}
function getLast(arr){
 let i = arr.length -1
  return arr[i];
}
function pushElement(arr){
  let el=1;
  arr.push(el);
  return arr;
}
function popElement(arr){
arr.pop();              
  return arr;
}
```
```javascript
//https://www.codewars.com/kata/5703c093022cd1aae90012c9/train/javascript
//Be Concise IV - Index of an element in an array
const  find = (array, element) => array.includes(element)
? array.indexOf(element) : "Not found";

```
```javascript
//https://www.codewars.com/kata/57d001b405c186ccb6000304/train/javascript
function iTri(s){
const dist = 2.4 + 112 + 26.2;
if (s === 0) return 'Starting Line... Good Luck!';
else if (s<2.4) return {'Swim': `${(dist - s).toFixed(2)} to go!` };
else if (s<114.4) return {'Bike': `${(dist - s).toFixed(2)} to go!` };  
else if (s< (dist-10)) return {'Run': `${(dist - s).toFixed(2)} to go!` };  
else if (s < dist) return {'Run':'Nearly there!'}; 
else return 'You\'re done! Stop running!'; 
}
```
```javascript
// https://www.codewars.com/kata/5a9e86705ee396d6be000091/train/javascript
function checkThreeAndTwo(arr) {
  const obj = {};
  for (let i = 0; i < arr.length; i++) {
  if (obj[arr[i]]) obj[arr[i]]++
  else obj[arr[i]] = 1;
  }
  for(let i in obj){
  if (obj[i] <2 || obj[i] >3) return false;
  }
  return true;
}
```
```javascript
//Regex Password Validation
//https://www.codewars.com/kata/52e1476c8147a7547a000811/train/javascript

function validate(p) {
 let long = p.length >=6; 
 let lower = !!p.match(/[a-z]/g);
 let upper = !!p.match(/[A-Z]/g);
 let num = !!p.match(/[0-9]/g);
 let sign = !p.match(/\W/g);
 return long && lower && upper && num && sign;
}
```
```javascript
//https://www.codewars.com/kata/59564f3bcc15b5591a00004a/train/javascript
//filterEvenLengthWords
function filterEvenLengthWords(words) {  //arr
  let arr = words.filter(el => el.length %2 === 0);
       return arr; 
       console.log(words);
}  
 
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```
```javascript
```


