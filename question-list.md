## Cracking Coding Interview

### Array and Strings

1. **Is Unique:** Implement an algorithm to determine if a string has all unique characters. What if you cannot use additional data structures?

2. **Check Permutation:** Given two strings, write a method to decide if one is a permutation of the other.

3. **URLify:** Write a method to replace all spaces in a string with '%20'. You may assume that the string has sufficient space at the end to hold the additional characters, and that you are given the "true" length of the string. (Note: if implementing in Java, please use a character array so that you can perform this operation in place.)
```
EXAMPLE
Input: "Mr John Smith ", 13
Output: "Mr%20John%20Smith
```

4. **Palindrome Permutation:** Given a string, write a function to check if it is a permutation of a palindrome. A palindrome is a word or phrase that is the same forwards and backwards. A permutation is a rearrangement of letters. The palindrome does not need to be limited to just dictionary words.
```
EXAMPLE
Input: Tact Coa
Output: True (permutations: "taco cat'; "atco eta·; etc.)
```

5. **One Away:** There are three types of edits that can be performed on strings: insert a character, remove a character, or replace a character. Given two strings, write a function to check if they are one edit (or zero edits) away.
```
EXAMPLE
pale, ple -> true
pales, pale -> true
pale, bale -> true
pale, bae -> false
```

6. **String Compression:** Implement a method to perform basic string compression using the counts of repeated characters. For example, the string aabcccccaaa would become a2blc5a3. If the "compressed" string would not become smaller than the original string, your method should return the original string.You can assume the string has only uppercase and lowercase letters (a - z).

7. **Rotate Matrix:** Given an image represented by an NxN matrix, where each pixel in the image is 4 bytes, write a method to rotate the image by 90 degrees. Can you do this in place?

8. **Zero Matrix:** Write an algorithm such that if an element in an MxN matrix is 0, its entire row and column are set to 0.

9. **String Rotation:** Assumeyou have a method isSubString() which checks if one word is a substring of another. Given two strings, s1 and s2, write code to check if s1 is a rotation of s2 using only one call to isSubString (e.g.,"waterbottle" is a rotation of"erbottlewat").


### Linked Lists

1. **Remove Dups:** Write code to remove duplicates from an unsorted linked list. How would you solve this problem if a temporary buffer is not allowed?

2. **Return Kth to Last:** Implement an algorithm to find the kth to last element of a singly linked list.

3. **Delete Middle Node:** Implement an algorithm to delete a node in the middle (i.e., any node but the first and last node, not necessarily the exact middle) of a singly linked list, given only access to that node.
```
EXAMPLE
lnput:the node c from the linked list a->b->c->d->e->f
Result: nothing is returned, but the new linked list looks like a ->b->d->e->f
```

4. **Partition:** Write code to partition a linked list around a value x, such that all nodes less than x come before all nodes greater than or equal to x. If x is contained within the list the values of x only need to be after the elements less than x (see below). The partition element x can appear anywhere in the "right partition"; it does not need to appear between the left and right partitions.
```
EXAMPLE
Input: 3 -> 5 -> 8 -> 5 -> 10 -> 2 -> 1 [partition= 5]
Output: 3 -> 1 -> 2 -> 10 -> 5 -> 5 -> 8
```

5. **Sum Lists:** You have two numbers represented by a linked list, where each node contains a single digit. The digits are stored in reverse order, such that the 1's digit is at the head of the list. Write a function that adds the two numbers and returns the sum as a linked list.
```
EXAMPLE
Input: (7-> 1 -> 6) + (5 -> 9 -> 2).That is,617 + 295.
Output: 2 -> 1 -> 9.That is,912.
```
*FOLLOW UP:* Suppose the digits are stored in forward order. Repeat the above problem.
```
Input: (6 -> 1 -> 7) + (2 -> 9 -> 5).That is,617 + 295.
Output: 9 -> 1 -> 2.That is, 912.
```

6. **Palindrome:** Implement a function to check if a linked list is a palindrome.

7. **Intersection:** Given two (singly) linked lists, determine if the two lists intersect. Return the intersecting node. Note that the intersection is defined based on reference, not value. That is, if the kth node of the first linked list is the exact same node (by reference) as the jth node of the second linked list, then they are intersecting.

8. **Loop Detection:** Given a circular linked list, implement an algorithm that returns the node at the beginning of the loop.
*DEFINITION: Circular linked list: A (corrupt) linked list in which a node's next pointer points to an earlier node, so as to make a loop in the linked list.*
```
EXAMPLE
Input:
Output:
SOLUTION
A - > B - > C - > D - > E - > C [the same C as earlier]
C
```


### Stacks and Queues

1. **Three in One:** Describe how you could use a single array to implement three stacks.

2. **Stack Min:** How would you design a stack which, in addition to push and pop, has a function min which returns the minimum element? Push, pop and min should all operate in 0(1) time.

3. **Stack of Plates:** Imagine a (literal) stack of plates. If the stack gets too high, it might topple. Therefore, in real life, we would likely start a new stack when the previous stack exceeds some threshold. Implement a data structure SetOfStacks that mimics this. SetOfStacks should be composed of several stacks and should create a new stack once the previous one exceeds capacity. SetOfStacks.push() and SetOfStacks. pop() should behave identically to a single stack (that is, pop() should return the same values as it would if there were just a single stack).
*FOLLOW UP: Implement a function popAt(int index) which performs a pop operation on a specific substack.*

4. **Queue via Stacks:** Implement a MyQueue class which implements a queue using two stacks.

5. **Sort Stack:** Write a program to sort a stack such that the smallest items are on the top. You can use an additional temporary stack, but you may not copy the elements into any other data structure (such as an array). The stack supports the following operations: push, pop, peek, and isEmpty.

6. **Animal Shelter:** An animal shelter, which holds only dogs and cats, operates on a strictly"first in, first out"basis. Peoplemustadopteitherthe"oldest"(basedonarrivaltime)ofallanimalsattheshelter, or they can select whether they would prefer a dog or a cat (and will receive the oldest animal of that type). They cannot select which speci c animal they would like. Create the data structures to maintain this system and implement operations such as enqueue, dequeueAny, dequeueDog, and dequeueCat. You may use the built in Linkedlist data structure.

### Trees and Graphs

1. **Route Between Nodes:** Given a directed graph, design an algorithm to find out whether there is a route between two nodes.

2. **Minimal Tree:** Given a sorted (increasing order) array with unique integer elements, write an algorithm to create a binary search tree with minimal height.

3. **List of Depths:** Given a binary tree, design an algorithm which creates a linked list of all the nodes at each depth (e.g., if you have a tree with depth D, you'll have D linked lists).

4. **Check Balanced:** Implement a function to check if a binary tree is balanced. For the purposes of this question, a balanced tree is defined to be a tree such that the heights of the two subtrees of any node never di er by more than one.

5. **Validate BST:** Implement a function to check if a binary tree is a binary search tree.

6. **Successor:** Write an algorithm to find the "next" node (i.e., in-order successor) of a given node in a binary search tree. You may assume that each node has a link to its parent.

7. **Build Order:* You are given a list of projects and a list of dependencies (which is a list of pairs of projects,wherethesecondprojectisdependentonthe rstproject).Allofaproject'sdependencies must be built before the project is. Find a build order that will allow the projects to be built. If there is no valid build order, return an error.
```
EXAMPLE
Input:
projects: a, b, c, d, e, f
dependencies: (a, d), (f, b), (b, d), (f, a), (d, c) 
Output:f, e, a, b, d, c
```

8. **First Common Ancestor:** Design an algorithm and write code to find the first common ancestor of two nodes in a binary tree. Avoid storing additional nodes in a data structure. 
*NOTE: This is not necessarily a binary search tree.*

9. **BST Sequences:** A binary search tree was created by traversing through an array from left to right and inserting each element. Given a binary search tree with distinct elements, print all possible arrays that could have led to this tree.
```
EXAMPLE
Input:
          2
        /   \
       1     3

Output: {2, 1, 3}, {2, 3, 1}
```

10. **Check Subtree:** T1 and T2 are two very large binary trees, with T1 much bigger thanT2. Create an algorithm to determine if T2 is a subtree of T1. A tree T2 is a subtree of T1 if there exists a node n in T1 such that the subtree of n is identical to T2. That is, if you cut off the tree at node n, the two trees would be identical.

11. **Random Node:** You are implementing a binary search tree class from scratch, which, in addition to insert, find, and delete, has a method getRandomNode() which returns a random node from the tree. All nodes should be equally likely to be chosen. Design and implement an algorithm for getRandomNode, and explain how you would implement the rest of the method.

12. **Paths with Sum:** You are given a binary tree in which each node contains an integer value (which might be positive or negative). Design an algorithm to count the number of paths that sum to a given value. The path does not need to start or end at the root or a leaf, but it must go downwards (traveling only from parent nodes to child nodes).


### Bit Manipulation

1. **Insertion:** You are given two 32-bit numbers, N and M, and two bit positions, i and j. Write a method to insert Minto N such that M starts at bit j and ends at bit i. You can assume that the bits j through i have enough space to fit all of M. That is, if M = 10011, you can assume that there are at least 5 bits between j and i. You would not, for example, have j = 3and i= 2, because M could not fully  t between bit 3 and bit 2.
```
EXAMPLE
Input: N 10000000000, M 10011, i = 2, j 6 
Output: N 10001001100
```

2. **Binary to String:** Given a real number between 0 and 1 (e.g., 0.72) that is passed in as a double, print the binary representation. If the number cannot be represented accurately in binary with at most 32 characters, print "ERROR".

3. **Flip Bit to Win:** You have an integer and you can flip exactly one bit from a O to a 1. Write code to find the length of the longest sequence of 1 s you could create.
```
EXAMPLE
Input: 1775 (or: 11011101111) 
Output: 8
```

4. **Next Number:** Given a positive integer, print the next smallest and the next largest number that have the same number of 1 bits in their binary representation.

5. **Debugger:** Explain what the following code does: ((n & (n-1)) == 0).

6. **Conversion: Write a function to determine the number of bits you would need to flip to convert integer A to integer B.
```
EXAMPLE
Input: 29 (or: 11101), 15 (or: 01111) 
Output: 2
```

7. **PairwiseSwap:** Write a program to swap odd and even bits in an integer with as few instructions as possible (e.g., bit O and bit 1 are swapped, bit 2 and bit 3 are swapped, and so on).

8. **Draw Line:** A monochrome screen is stored as a single array of bytes, allowing eight consecutive pixels to be stored in one byte. The screen has width w, where w is divisible by 8 (that is, no byte will be split across rows). The height of the screen, of course, can be derived from the length of the array and the width. Implement a function that draws a horizontal line from (xl, y) to (x2, y).

The method signature should look something like:
```
drawLine(byte[] screen, int width, int xl, int x2, int y)
```


### Math and Logic Puzzles

1. **The Heavy  Pill:** You have 20 bottles of pills. 19 bottles have 1.0 gram pills, but one has pills of weight 1.1 grams. Given a scale that provides an exact measurement, how would you find the heavy bottle? You can only use the scale once.

2. **Basketball:** You have a basketball hoop and someone says that you can play one of two games.
```
Game 1: You get one shot to make the hoop.
Game 2: You get three shots and you have to make two of three shots.
```
If p is the probability of making a particular shot, for which values of p should you pick one game or the other?

3. **Dominos:** There is an 8x8 chessboard in which two diagonally opposite corners have been cut off. You are given 31 dominos, and a single domino can cover exactly two squares. Can you use the 31 dominos to cover the entire board? Prove your answer (by providing an example or showing why it's impossible).

4. **Ants on a Triangle:** There are three ants on different vertices of a triangle. What is the probability of collision (between any two or all of them) if they start walking on the sides of the triangle? Assume that each ant randomly picks a direction, with either direction being equally likely to be chosen, and that they walk at the same speed.
*Similarly, finnd the probability of collision with n ants on an n-vertex polygon.*

5. **Jugs of Water:** You have a five-quart jug, a three-quart jug, and an unlimited supply of water (but no measuring cups). How would you come up with exactly four quarts of water? Note that the jugs are oddly shaped, such that  lling up exactly "half" of the jug would be impossible.

6. **Blue-Eyed Island:** A bunch of people are living on an island, when a visitor comes with a strange order: all blue-eyed people must leave the island as soon as possible. There will be a flight out at 8:00pm every evening. Each person can see everyone else's eye color, but they do not know their own (nor is anyone allowed to tell them). Additionally, they do not know how many people have blue eyes, although they do know that at least one person does. How many days will it take the blue-eyed people to leave?

7. **The Apocalypse:** In the new post-apocalyptic world, the world queen is desperately concerned about the birth rate. Therefore, she decrees that all families should ensure that they have one girl or else they face massive fines. If all families abide by this policy-that is, they have continue to have children until they have one girl, at which point they immediately stop-what will the gender ratio of the new generation be? (Assume that the odds of someone having a boy or a girl on any given pregnancy is equal.) Solve this out logically and then write a computer simulation of it.

8. **The Egg Drop Problem:** There is a building of 100 floors. If an egg drops from the Nth floor or above, it will break. If it's dropped from any floor below, it will not break.You're given two eggs. Find N, while minimizing the number of drops for the worst case.

9. **100 Lockers:** There are 100 closed lockers in a hallway. A man begins by opening all 100 lockers. Next, he closes every second locker. Then, on his third pass, he toggles every third locker (closes it if it is open or opens it if it is closed). This process continues for 100 passes, such that on each pass i, the man toggles every ith locker. After his 100th pass in the hallway, in which he toggles only locker
#100, how many lockers are open?

10. **Poison:** You have 1000 bottles of soda, and exactly one is poisoned. You have 10 test strips which can be used to detect poison. A single drop of poison will turn the test strip positive permanently. You can put any number of drops on a test strip at once and you can reuse a test strip as many times as you'd like (as long as the results are negative). However, you can only run tests once per day and it takes seven days to return a result. How would you figure out the poisoned bottle in as few days as possible?
*Follow up: Write code to simulate your approach.*


### Object-Oriented Design

1. **Deck of Cards:** Design the data structures for a generic deck of cards. Explain how you would subclass the data structures to implement blackjack.

2. **Call Center:** Imagine you have a call center with three levels of employees: respondent, manager, and director. An incoming telephone call must be  rst allocated to a respondent who is free. If the respondent can't handle the call, he or she must escalate the call to a manager. If the manager is not free or not able to handle it, then the call should be escalated to a director. Design the classes and data structures for this problem. Implement a method dispatchCall () which assigns a call to the first available employee.

3. **Jukebox:** Design a musical jukebox using object-oriented principles.

4. **Parking Lot:** Design a parking lot using object-oriented principles.

5. **Online Book Reader:** Design the data structures for an online book reader system.

6. **Jigsaw:** Implement an NxN jigsaw puzzle. Design the data structures and explain an algorithm to solve the puzzle. You can assume that you have a fitsWith method which, when passed two puzzle edges, returns true if the two edges belong together.

7. **Chat Server:** Explain how you would design a chat server. In particular, provide details about the various backend components, classes, and methods. What would be the hardest problems to solve?

8. **Othello:** Othello is played as follows: Each Othello piece is white on one side and black on the other. When a piece is surrounded by its opponents on both the left and right sides, or both the top and bottom, it is said to be captured and its color is flipped. On your turn, you must capture at least one of your opponent's pieces. The game ends when either user has no more valid moves. The win is assigned to the person with the most pieces. Implement the object-oriented design for Othello.

9. **Circular Array:** Implement a CircularArray class that supports an array-like data structure which can be e iciently rotated. If possible, the class should use a generic type (also called a template), and should support iteration via the standard for (Obj o : circularArray) notation.

10. **Minesweeper:** Design and implement a text-based Minesweeper game.

11. **File System:** Explain the data structures and algorithms that you would use to design an in-memory file system. Illustrate with an example in code where possible.

12. **Hash Table:** Design and implement a hash table which uses chaining (linked lists) to handle collisions.


### Recursion and Dynamic Programming

1. **Triple Step:** A child is running up a staircase with n steps and can hop either 1 step, 2 steps, or 3 steps at a time. Implement a method to count how many possible ways the child can run up the stairs.

2. **Robot in a Grid:** Imagine a robot sitting on the upper left corner of grid with r rows and c columns. The robot can only move in two directions, right and down, but certain cells are "off limits" such that the robot cannot step on them. Design an algorithm to find a path for the robot from the top left to the bottom right.

3. **Magic Index: A magic index in an array A[0..n-1] is defined to be an index such that A[i] = i. Given a sorted array of distinct integers, write a method to find a magic index, if one exists, in array A.
*FOLLOW UP: What if the values are not distinct?*

4. **Power Set:** Write a method to return all subsets of a set.

5. **Recursive Multiply:** Write a recursive function to multiply two positive integers without using the * operator (or / operator). You can use addition, subtraction, and bit shifting, but you should minimize the number of those operations.

6. **Towers of Hanoi: In the classic problem of the Towers of Hanoi, you have 3 towers and N disks of di erent sizes which can slide onto any tower. The puzzle starts with disks sorted in ascending order of size from top to bottom (i.e., each disk sits on top of an even larger one). You have the following constraints:
```
(1) Only one disk can be moved at a time.
(2) A disk is slid off the top of one tower onto another tower.
(3) A disk cannot be placed on top of a smaller disk.
```
Write a program to move the disks from the first tower to the last using Stacks.

7. **Permutations without Dups:** Write a method to compute all permutations of a string of unique characters.

8. **Permutations with Duplicates:** Write a method to compute all permutations of a string whose characters are not necessarily unique. The list of permutations should not have duplicates.

9. **Parens:** Implement an algorithm to print all valid (i.e., properly opened and closed) combinations of n pairs of parentheses.
```
EXAMPLE
Input: 3
Output: ((())), (()()), (())(), ()(()), ()()()
```

10. **Paint Fill:** Implement the "paint fill" function that one might see on many image editing programs. That is, given a screen (represented by a two-dimensional array of colors), a point, and a new color, fill in the surrounding area until the color changes from the original color.

11. **Coins:** Given an infinite number of quarters (25 cents), dimes (1O cents), nickels (5 cents), and pennies (1 cent), write code to calculate the number of ways of representing n cents.

12. **Eight Queens:** Write an algorithm to print all ways of arranging eight queens on an 8x8 chess board so that none of them share the same row, column, or diagonal. 

13. **Stack of Boxes:** You have a stack of n boxes, with widths wi, heights hi, and depths di. The boxes cannot be rotated and can only be stacked on top of one another if each box in the stack is strictly larger than the box above it in width, height, and depth. Implement a method to compute the height of the tallest possible stack. The height of a stack is the sum of the heights of each box.

14. **Boolean Evaluation:** Given a boolean expression consisting of the symbols 0(false), 1(true), &(AND), |(OR), and ^(XOR), and a desired boolean result value result, implement a function to count the number of ways of parenthesizing the expression such that it evaluates to result. The expressionshouldbefullyparenthesized(e.g.,(0)A(1))butnotextraneously(e.g.,(((0))^(1))).
```
EXAMPLE
countEval("1^0|0|1", false) -> 2 
countEval("0&0&0&1^1|0", true)-> 10
```

### System Design and Scalability

1. **Stock Data:** Imagine you are building some sort of service that will be called by up to 1,000 client applications to get simple end-of-day stock price in rmation (open, close, high, low). You may assume that you already have the data, and you can store it in any format you wish. How would you design the client-facing service that provides the information to client applications? You are responsible  r the development, rollout, and ongoing monitoring and maintenance of the feed. Describe the different methods you considered and why you would recommend your approach. Your service can use any technologies you wish, and can distribute the information to the client applications in any mechanism you choose.

### Sorting and Searching

1. **Sorted Merge:** You are given two sorted arrays, A and B, where A has a large enough buffer at the end to hold B. Write a method to merge B into A in sorted order.

### Testing

### Databases

### Threads and Locks

### C/C++ Related

### Java Related

