## Answers

**Question 1:** `cutoff` is not a parameter in the `playTurn` method because it is instantiated by the constructor. Member variables are accessable by methods of the class which contains them.

**Question 2:** 

 `ScoreSheet s = new ScoreSheet(); System.out.println(s.getTurnAverage()); `

Running this code would print the average score as a double. By call the `getTurnAverage` method right after creating a new ScoreSheet object, the code will print out '0.0' by default.

**Question 3:**  The `numBusts` variable could be incremented in the `playTurn` method. In this method, we check the three cases that would end a turn, one of which is rolling a 1. This would be a good place to increment the `numBusts` variable without affecting the results.

**Question 4:** Based on my current understanding of the code I think that the error would lie in the while loops in the `PigGame` class's `playGame` or `playTurn` method. I am fairly certain that the error does not lie in any of the Query methods because they don't change data.

**Question 5:** The problem with the program was that the `roll` method in the `Die` class would always would always give `upValue` '0' because of a type casting error. Because of this `playGame` method in the `PigGame` class would never reach '100' resulting in an infinite loop. To fix the error, I changed the code to:

`upValue = ((int)(Math.random() * 6)) + 1;`

**Question 6:** 

10: 5.67

15: 6.44

20: 5.72

25: 6.34






 
 