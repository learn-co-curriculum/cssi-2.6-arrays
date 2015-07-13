---
tags: cssi, javascript
level: 1
languages: javascript
---
#Arrays
After the lesson, you'll understand:
+ What an array is
+ js array syntax
+ assigning an array to a variable
+ array indexing
+ how to locate and identify data in an array
+ how to change an array entry
+ calling methods on an array - finding the length of an array

We’ve learned how to store a piece of data in a variable.

```
>var student = "Tamara"
```

If we want to store a whole list of data, we need to make an array. Arrays are a type of data structure that creates an ordered list of individual elements.

One example of a real world array is a grocery list. Each item on the list has an index (number) and a element (food item). Another example would be a parking lot: each space is numbered (index) and contains a car (element).

You can visualize an array as a two-column table where the left column is the index (or the order) and the right column is the thing you’re listing:

| Index | Value     |
|-------|-----------|
| 0     | "Bread" |
| 1     | "Cheese"   |
| 2     | "Milk"  |
| 3     | "Apples"   |
| 4     | "Eggs"     |

Notice that the index starts at 0. The first item in an array has index 0, the second has index 1, and so forth. 



We saw this same index numbering when we used methods to identify characters in a string earlier. In fact, you can think of a string like an array of characters.

Let’s initialize an array for our students:
```
>var students= ['Tamara','Georgia','Norah','Joseph','Nicki','Rob']
>students
["Tamara", "Georgia", "Norah", "Joseph", "Nicki", "Rob"]
```
Square brackets `[ ]` denote the contents of an array. An array can contain any combination of data types.  An array can be stored in a variable just like a number or string.
You'll notice that we don't write the index of the elements anywhere. The computer _automatically_ makes an index starting at 0 and incrementing by 1 for each element.

## Accessing and Modifying Elements
To access an element of an array, just call the name of your array variable and the index that the element is at.
```
>students[3]
< "Joseph"
```

What if we wanted to reassign an element in an array? What if Joseph dropped the class, and instead we had Barry?
```
>students[3] = 'Barry'
>students[3]
< "Barry"
```
The array element at index three has been changed!

Just like we got the length for our strings with a string method, we can also get the length of an array. Every array has a property that is it's length, which we can access with the '.'
```
>console.log(students.length);
```
This prints out '6' since our students array contains 6 elements. (Notice though that the last element of our array only has an index of '5', this will become important when discussing loops.)

##Add and Remove items from an array
We can also add and remove items from an array. Arrays actually have methods built in to them. Remember that methods are just a set of instructions.
```
names.push("Alfred")
```
`push` will add an item to the end of the array. In this case, the argument is "Alfred" and the array is names.

```
var lastName = names.pop()
```
`pop` will remove the last item in an array and return it. Since we just added "Alfred" to the end, that is what names.pop() returns.

Here are some other cool methods to experiment with: .sort(), .splice(), .split()
