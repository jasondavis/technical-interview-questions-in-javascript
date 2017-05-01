# technical-interview-in-javascript
This is just private note for my interview. If you found this repo by googling, please check below awesome links instead.

* https://github.com/MaximAbramchuck/awesome-interview-questions#javascript
* https://github.com/kennymkchan/interview-questions-in-javascript
* https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015

## Check List

* Time or Space Complexity
* Recursive
* String
* Array
* Map / Set
* Linked List
* Stack / Queue
* Tree
* Sort
* Search

## Time or Space Complexity

* O(1) -> Constant
* O(n) -> Linear
* O(n^2) n power of 2
* O(log n) -> Binary Search 
* O(n log n)

* http://stackoverflow.com/questions/1592649/examples-of-algorithms-which-has-o1-on-log-n-and-olog-n-complexities

## Javascript Class Example

```javascript
class Queue {
  constructor() {
    this.stack1 = [];
    this.stack2 = [];
  }

  enqueue(input) {
    this.stack1.push(input);
  }

  dequeue() {
    while(this.stack1.length > 0) {
      this.stack2.push(this.stack1.pop());
    }
    return this.stack2.pop();
  }
}
```

## String

```javascript
str.length
str.charAt(i)
str.split('').reverse().join('')
```

## Set

```javascript
let set = new Set();
set.add(1); // [1]
set.add(1): // still [1]
```

## Map

```javascript
let map = new Map();
map.set('key', 'value');
map.get('key');
map.has('key');
```

## Stack

```javascript
let stack = [];
stack.push(1);
stack.pop();
```

## Queue

```javascript
let queue = [];
queue.push(1);
queue.push(2);
let dequeue = queue.shift(); //it is slow
// *peek : get the item at the front of the queue without dequeuing it
```