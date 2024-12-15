# ActionScript 3 ArrayIndexOutOfBoundsException Bug
This repository demonstrates a common ActionScript 3 error: `ArrayIndexOutOfBoundsException`. This occurs when you try to access an element in an array using an index that is outside the valid range of indices (0 to array.length - 1).

## Bug Description
The `bug.as` file contains a function that attempts to access `myArray[10]`. If `myArray` has fewer than 11 elements, this will throw an `ArrayIndexOutOfBoundsException`.  This is a runtime error that crashes your application.

## Solution
The `bugSolution.as` file provides a solution by adding a check to ensure the index is within the valid range before accessing the array element.

## How to Reproduce
1. Clone this repository.
2. Open `bug.as` in an ActionScript 3 IDE (like FlashDevelop).
3. Create an array `myArray` with fewer than 11 elements.
4. Run the `myFunction()` function.  You will observe the `ArrayIndexOutOfBoundsException`.
5. Now, run the `myFunction()` from the `bugSolution.as` file. This version will gracefully handle the situation, preventing the error.