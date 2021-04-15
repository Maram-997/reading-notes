# Comparison  And Logical Operators 
* You can evaluate a situation by comparing one value in the script to what you expect it might be. The results will be a Booleans: TRUE or FALSE.
- (==) is equal to, so here we comparing the values.
- (!=) not equal to.
- (===) strict equal to, this compares the two values and the datatype.
- (!==) strict not equal to, compares the values and their datatype if they are not the same and every value can be treated as true or false even if it is not a Boolean.
 - (>) greater than; checks if the number on the left is greater the the number on right.
 - (<) less than; checks if the number on the left is lesser the the number on right.
 - (>=) great than or equal; checks if the number on the left is greater or equal to the the number on right.
 -(<=) less than or equal to; checks if the number on the left is lesser than or equal to  the the number on right.



 #### Logical operators allows you to compare the result of more than one comparison operator. ((5<2)&& (2>=3)), so this contains three expressions; the first is (5<2) it's false condition. the second expression is (2>=3) and it returns false too. So the third expression is the logical operator, it checks if both sides are true, but as it seems they are not, so it returns false.

 ### The Three Types of logical operators:
 * The logical and (&&) ; both sides should be true otherwise it returns false.
 * The logical or (||) ; one of the sides should be true at least to return as true. else it return false.
 * The logical not (!) ; this is unlike the first two, it takes one single Boolean value and convert it. like: !(2<1) the result is true.


  ### Loops 
  loops keep running the codes as long as the condition is true. So it repeats until the condition returns false.
  
  ### The three common types of loops:
  1.For:
  If you need to run code a specific number of times, use loop for and the condition is usually a counter which is used to tell how many times the loop should run.

  2.While:
  If you do not know how many this code should run. So the code will continue to loop as long as the condition is true.

  3.Do While.


  ### The three statement the condition is made up of:
  * Initialization (i) : it acts as the counter.
  * Condition : the loop should continue to run until the counter reaches a specified number.
  * update : everything the loop has run the statement in curly braces, it add one by one to the counter (i++).

  ### Three important things to know while using loops:
  - Keyword  
  1.Break: it ends the loop of the codes and goes to the next statement.
  2.Continue: to keep the current iteration.
  - Loops and arrays: 
  once the loop has run the right number of times, the loop stops.
  - Performance:
  if the condition never returns false, you get what is commonly reffered to as an infinite loop.
  
