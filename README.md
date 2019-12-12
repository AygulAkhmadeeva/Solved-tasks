# Solved-tasks
* task 1
```javascript
let a = 1;
let b= 2;
console.log(a+b);
```
```javascript
//://www.codewars.com/kata/is-he-gonna-survive/train/javascript
//Is he gonna survive?
function hero(bullets, dragons){
return dragons*2 <= bullets ;
}
```
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