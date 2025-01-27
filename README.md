# Kotlin's removeIf() Gotcha: Mutable vs Immutable Collections

This repository showcases a common pitfall in Kotlin when working with collections and the `removeIf()` function.  The `removeIf()` function is designed for modifying mutable collections (like `MutableList`, `MutableSet`, `MutableMap`).  Attempting to use it with immutable collections (like `List`, `Set`, `Map`) will lead to a compile-time error.

The `bug.kt` file demonstrates the correct usage with mutable collections and highlights the error that occurs when attempting to use `removeIf()` with an immutable collection.  The solution file (`bugSolution.kt`) offers no changes as the main file correctly demonstrates the bug.

## How to Reproduce

1. Clone this repository.
2. Open `bug.kt` in a Kotlin IDE.
3. Observe the successful modification of mutable collections and the compile-time error when using `removeIf()` with an immutable collection.
