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