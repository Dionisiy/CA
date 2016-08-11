

- What will happen if an infinite while loop is run in Javascript?

**Answer**: The program will crash

- Which of the following is an infinite loop?

```
//one
var i = 1; 
while(i < 4) {
  console.log("loading…");
  i = i + 1
};
//two
var i = 1;
while(i == 4) {
  console.log("loading…");
};
//three
var i = 1;
while(i == 4) {
  console.log("loading…");
  i = i + 1
}
//four
var i = 1;
while(i < 4) {
  console.log("loading…");
};
```
**Answer**: four

- What should the blank line be replaced with to properly exit what is currently an infinite loop?

```
var check = true;var loopCheck = function(check){

 while(check){

 console.log("Looped once!");

 ____________

 }

}
```

**Answer**: check = false;
