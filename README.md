# Solved-tasks
* Is he gonna survive?
```javascript
//www.codewars.com/kata/is-he-gonna-survive/train/javascript
function hero(bullets, dragons){
return dragons*2 <= bullets ;
}
```
* Breaking chocolate problem
```javascript
//www.codewars.com/kata/breaking-chocolate-problem/train/javascript
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
* Well of Ideas - Easy Version
```javascript
//www.codewars.com/kata/well-of-ideas-easy-version/train/javascript
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
* Merge two sorted arrays into one
```javascript
//www.codewars.com/kata/merge-two-sorted-arrays-into-one/train/javascript
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
* Return the closest number multiple of 10
```javascript
//www.codewars.com/kata/return-the-closest-number-multiple-of-10/train/javascript
const closestMultiple10 = num => {
console.log(num);
 if (num%10 < 5) return num - (num %10);
 if (num%10 >= 5) return num + 10 - num % 10;
};
```
* Area of a Square
```javascript
//www.codewars.com/kata/area-of-a-square/train/javascript
function squareArea(A){
console.log(A);
const cu = 4*A*A/(Math.PI*Math.PI)
return +cu.toFixed(2);
  }
```
* Calculate Two People's Individual Ages #7
```javascript
//www.codewars.com/kata/calculate-two-peoples-individual-ages/train/javascript
function getAges(s,d){
console.log(s,d);
if (s<0 || d<0 || d>s) return null;
const arr = [];
arr[1] = (s-d)/2;
arr[0] = arr[1]+d;
return arr;
};
```
* Is this a triangle? #7
```javascript
//www.codewars.com/kata/is-this-a-triangle/train/javascript
function isTriangle(a,b,c) {
 return (a + b > c && a + c > b && b + c > a);
 }
```
* Power of two
```javascript
//www.codewars.com/kata/power-of-two/train/javascript
let isPowerOfTwo = (n) => !(n & (n - 1)) && n != 0;
```
* 7 kyu Factorial
```javascript
//www.codewars.com/kata/factorial-1/train/javascript
function factorial(n){
if (n === 0) return 1;
return n*factorial(n-1);
}
```
* Filter the number #7
```javascript
//www.codewars.com/kata/filter-the-number/train/javascript
var FilterString = function(value) {
  //Complete this function :)
}
var FilterString = function(value) {
console.log(value);
  let mV = value.split('');
  let res = mV.filter((j) => j >= 0); //massiv s chislami
  return +res.join('');
  }
const FilterString = value => {
  return Number(
    value
      .split("")
      .filter(ele => Number(ele) == ele)
      .join("")
  );
}; //&& isNaN(value[i])
```

* Square Every Digit #7
```javascript
//www.codewars.com/kata/square-every-digit/train/javascript
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
* Enumerable Magic #1 - True for All?
```javascript
//www.codewars.com/kata/enumerable-magic-number-1-true-for-all/train/javascript
function all( arr, fun ) {
  for(let i = 0; i < arr.length; i++) {
    if(!fun(arr[i])) {
      return false;
    }
  }
  return true;
}
```
* Find the next perfect square!   7rank
```javascript
//https://www.codewars.com/kata/find-the-next-perfect-square/train/javascript
const findNextSquare = (sq) => (Math.sqrt(sq) % 1 === 0) ?((Math.sqrt(sq)+1)*(Math.sqrt(sq)+1)) : -1;
```

* How many times should I go? #7
```javascript
//www.codewars.com/kata/57efcb78e77282f4790003d8/solutions/javascript
function howManyTimes(annualPrice, individualPrice) {
  return Math.ceil(annualPrice / individualPrice);
}
```
* Every possible sum of two digits #7
```javascript
//www.codewars.com/kata/every-possible-sum-of-two-digits/train/javascript
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
* Formatting decimal places #1
```javascript
//www.codewars.com/kata/formatting-decimal-places-number-1/train/javascript
function twoDecimalPlaces(number) {
return Math.trunc(number*100)/100;
}
```
* Tortoise racing, rank #6
```javascript
//www.codewars.com/kata/tortoise-racing/train/javascript
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
* Binary Addition
```javascript
//www.codewars.com/kata/binary-addition/train/javascript
const addBinary = (a,b) => (a+b).toString(2);
```
* Hex to Decimal
```javascript
//www.codewars.com/kata/hex-to-decimal/train/javascript
function hexToDec(hexString){
return parseInt(hexString, 16);
}
```
* Is every value in the array an array?
```javascript
//www.codewars.com/kata/582c81d982a0a65424000201/train/javascript
const arrCheck = value => {
for (let i = 0; i < value.length; i++){
if ( Array.isArray(value[i])  ) continue;
else return false;
} return true;
}
```
* Find the first non-consecutive number
```javascript
//www.codewars.com/kata/58f8a3a27a5c28d92e000144/train/javascript
function firstNonConsecutive (arr) {
console.log(arr);               
for (let i = 0; i < arr.length-1;i++){ 
    if ( arr[i+1] - arr[i] !== 1 ){                    
    return arr[i+1];                         
    }
  }  return null;
}
```

*Enumerable Magic #3 - Does My List Include This?
```javascript
//www.codewars.com/kata/545991b4cbae2a5fda000158/solutions/javascript
const include = (arr, item) => arr.includes(item);
```
* Odd or Even?
```javascript
function oddOrEven(arr) {
let sum = 0;                           
for (let i = 0; i < arr.length; i++){  
  sum += arr[i];                  
}
if (sum %2 === 0) {
return 'even';
} else {
return 'odd';
}
}
```
* Remove the minimum
```javascript
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

* Find the divisors! Cata7
```javascript
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
* Training JS #4: Basic data types--Array
```javascript
//www.codewars.com/kata/571effabb625ed9b0600107a/train/javascript
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

* Be Concise IV - Index of an element in an array
```javascript
//www.codewars.com/kata/5703c093022cd1aae90012c9/train/javascript
const  find = (array, element) => array.includes(element)
? array.indexOf(element) : "Not found";
```


```javascript
//www.codewars.com/kata/57d001b405c186ccb6000304/train/javascript
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
//www.codewars.com/kata/5a9e86705ee396d6be000091/train/javascript
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
* Regex Password Validation
```javascript
//www.codewars.com/kata/52e1476c8147a7547a000811/train/javascript
function validate(p) {
 let long = p.length >=6; 
 let lower = !!p.match(/[a-z]/g);
 let upper = !!p.match(/[A-Z]/g);
 let num = !!p.match(/[0-9]/g);
 let sign = !p.match(/\W/g);
 return long && lower && upper && num && sign;
}
```

* filterEvenLengthWords
```javascript
//https://www.codewars.com/kata/59564f3bcc15b5591a00004a/train/javascript
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


