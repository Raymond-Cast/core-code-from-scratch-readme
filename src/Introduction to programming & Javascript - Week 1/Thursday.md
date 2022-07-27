# Challenges
___

## **1. Print special numbers**

Print all the even numbers in the range of numbers from 0 to 100 using Flow Control Structure. 

### **For**

```java
for (let i = 0; i <= 100; i++) {
    if (i % 2 == 0) {
        console.log(i);
    }
}
```

## **2. Bad Code Exercise**

The code shown below is not working in the right way, as a task you must find the error made by the developer who programmed this code and correct it, for this exercise you must explain what the error is and place the correct code

**Explanation** 

The error in the BAD Code is caused because it was treated as an assignment instead of a comparision. 'cond' was assigned the value 'true', so when running the 'IF' conditional there were no value to compare with, as it was re-written/re-assigned to TRUE.

### **BAD Code**

```java
var cond = false;

if ((cond = true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```

### **GOOD Code**

```java
var cond = false;

if ((cond == true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```

### **BAD Code 2***

#### **Description**

You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly

```java
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
}
if (n < 1000) {
  console.log('');
} else {
  console.log('Just a regular number');
}
if (n % 10 == 0) {
  console.log('This number is multiple of 10');
}
```

### **GOOD Code**

```java

var n = 100;

if (n == 100) {
  console.log('This is a special number!');
} else {
    if ((n < 1000) && (n % 10 == 0)) {
    console.log('');
    } else {
  console.log('Just a regular number');
}
}
```