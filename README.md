# ConcurrentModificationException in Java

This repository demonstrates a common Java error: the `ConcurrentModificationException`.  The `ConcurrentModificationExceptionExample.java` file contains code that throws this exception. The solution, `ConcurrentModificationExceptionExampleSolution.java`, provides a corrected version.

## Description

The `ConcurrentModificationException` occurs when you modify a collection (like an ArrayList) while iterating over it using an iterator that doesn't support concurrent modification. The for-each loop implicitly uses an iterator that is not fail-fast, leading to this exception. 

## Solution

The solution demonstrates the proper way to modify a list while iterating: using an `Iterator` and its `remove()` method.