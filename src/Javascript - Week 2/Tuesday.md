# Challenges
___

## 1. Start this [HTML](https://edpuzzle.com/join/vawasaj) course
___

## 2. Multiply exercise
___

This code does not execute properly. Try to figure out why.


```javascript

function multiply(a, b){
  a * b
}
```
### Solution(s)

```javascript

function multiply(a,b) {
    return a*b;
}
```

```javascript

function multiply(a, b){
  let c = a * b
  return c;
}
```

## 3. ASCII Total
___

You'll be given a string, and have to return the sum of all characters as an int. The function should be able to handle all ASCII characters.

examples:

uniTotal("a") == 97 uniTotal("aaa") == 291


```javascript

function uniTotal (string) {
  let length = string.length;
  let sum = 0;
  for (let i = 0; i < length; i++) {
    sum = sum + string.charCodeAt(i);
  }
  return sum;
}
```