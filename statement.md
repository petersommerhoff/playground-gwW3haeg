# Functional Programming in Kotlin

This is a hands-on guide to Kotlin's main functional programming features:

1. Higher-order functions
1. Lambda expressions
1. Lambdas with Receivers
1. Lazy Evaluation


## Functions in Kotlin

Before talking about higher-order functions and lambdas, I want to first get everyone on the same page when it comes to first-order (normal) functions.


### Function Declaration

In its most explicit form, a function declaration in Kotlin looks like this:

```kotlin runnable
fun modifyString(str: String): String {
    return str.toUpperCase()
}
```

