```
//For Each ======== 
string[] states = { "Alabama", "Alaska", "Arizona", "Arkansas", "California", "Colorado" };
  foreach (string state in states) {

// The `state` variable takes on the value of an element in `states` and updates every iteration.
  Console.WriteLine(state);
}
// Will print each element of `states` in the order they appear in the array. 

// While Loop =======
string guess = "";
Console.WriteLine("What animal am I thinking of?");
 
// This loop will keep prompting the user, until they type in "dog".
while (guess != "dog") {
  Console.WriteLine("Make a guess:");
  guess = Console.ReadLine();
}
Console.WriteLine("That's right!");


//DO While
do {
  DoStuff();
} while(boolCondition);
 
// This do-while is equivalent to the following while loop.
 
DoStuff();
while (boolCondition) {
  DoStuff();
}


// Jump Statements
while (true) {
  Console.WriteLine("This prints once.");
  // A `break` statement immediately terminates the loop that contains it.
  break;
}
 
for (int i = 1; i <= 10; i++) {
  // This prints every number from 1 to 10 except for 7.
  if (i == 7) {
    // A `continue` statement skips the rest of the loop and starts another iteration from the start.
    continue;
  }
  Console.WriteLine(i);
}
 
static int WeirdReturnOne() {
  while (true) {
    // Since `return` exits the method, the loop is also terminated. Control returns to the method's caller.
    return 1;
  }
}



```
