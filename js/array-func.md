# 数组方法
------
#### **# push(element, ...)**
> * `参数`：
         element：
         ...：
> * `用法`：
        向数组的末尾添加一个或多个元素，并返回新的长度
```
let arr = new Array('George', 'John', 'Thomas');
console.log(arr);               // ['George', 'John', 'Thomas']
console.log(arr.push('James')); // 4   arr 的新长度
console.log(arr);               // ['George', 'John', 'Thomas', 'James']
```
#### **# pop()**
> * `参数`：
        无
> * `用法`：
        pop() 方法将删除数组的最后一个元素，把数组长度减 1，并且返回它删除的元素的值。如果数组已经为空，则 pop() 不改变数组，并返回 undefined 值。
```
let arr = new Array('George', 'John', 'Thomas');
console.log(arr);           // ['George', 'John', 'Thomas']
console.log(arr.pop());     // 'Thomas'
console.log(arr);           // ['George', 'John']
```
#### **# shift()**
> * `参数`：
        无
> * `用法`：
        shift() 返回数组原来的第一个元素的值；如果数组是空的，那么 shift() 方法将不进行任何操作，返回 undefined 值。
```
let arr = new Array('George', 'John', 'Thomas');
console.log(arr);           // ['George', 'John', 'Thomas']
console.log(arr.shift());   // 'George'
console.log(arr);           // ['John', 'Thomas']
```
#### **# unshift(element, ...)**
> * `参数`：
         element：
         ...：
> * `用法`：
        unshift() 方法将把它的参数插入数组的头部，并将已经存在的元素顺次地移到较高的下标处，以便留出空间。
```
let arr = new Array('George', 'John', 'Thomas');
console.log(arr);                       // ['George', 'John', 'Thomas']
console.log(arr.unshift('William'));    // 4   arr 的新长度
console.log(arr);                       // ['William', 'George', 'John', 'Thomas']
```
#### **# forEach(function(currentValue, index, arr), thisValue)**
> * `参数`：
```
         currentValue：数组中正在处理的当前元素。   
         index：数组中正在处理的当前元素的索引。   
         arr：forEach() 方法正在操作的数组。   
         thisValue：当执行回调函数时用作 this 的值(参考对象)。
```
> * `用法`：
        forEach() 方法用于调用数组的每个元素，并将元素传递给回调函数，forEach() 对于空数组是不会执行回调函数的。
```
let arr = ['George', 'John', 'Thomas'];
let copy = [];
arr.forEach(item => copy.push(item));
console.log(copy) // ['George', 'John', 'Thomas']
```






#### **# filter(，)**
#### **# find(，)**
#### **# map(，)**
#### **# reduce(，)**
#### **# reduceRight(，)**
#### **# some(，)**
#### **# every(，)**
#### **# splice(，)**
#### **# join(，)**
#### **# slice(，)**
#### **# concat(，)**
#### **# indexOf(，)**
#### **# lastIndexOf(，)**
#### **# reverse(，)**
#### **# sort(，)**