# Unexpected Behavior of removeIf on MutableList and MutableSet in Kotlin

This code demonstrates an uncommon bug related to the `removeIf` function in Kotlin when used with mutable lists and sets.  The issue arises from modifying the collection while iterating over it using `removeIf`.

The `removeIf` function is designed to remove elements that satisfy a given predicate. However, when used with a predicate that modifies the collection's structure during the iteration, the behavior might become unpredictable.  The example shows how `removeIf` on `MutableList` and `MutableSet` differ in this case, leading to potential unexpected outputs and application errors. The solution provides safer alternatives for these scenarios.