### While syntax

The while loop is ideal when you want to use a loop, but you don't know how many times you'll have to execute that loop.


As long as the condition evaluates totrue, the loop will continue to run. As soon as it's false, it'll stop. (When you use a number in a condition, as we did earlier, JavaScript understands 1 to mean true and 0 to mean false.)

###A fellow of infinite loops

We mentioned infinite loops in the previous exercise. If you give a whileloop a condition that is true and you don't build in a way for that condition to possibly become false, the loop will go on forever and your program will crash. No good!

To prevent this from happening, youalways need a way to ensure the condition between your whileparentheses can change.

You'll see the same code from the last exercise in the editor to the right, only we've taken out the part that changes the loop's condition.


You may have noticed that when we give a variable the boolean value true, we check that variable directly—we don't bother with ===. For instance,


`
var bool = true;
while(bool){
    //Do something
}
`

is the same thing as

```
var bool = true;

   while(bool === true)

{ //Do something }

```
but the first one is faster to type. Get in the habit of typing exactly as much as you need to, and no more!

