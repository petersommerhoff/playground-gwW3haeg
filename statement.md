# Breaking Kotlin



## Breaking the Compiler

As you know, you don't normally need to end all statements and expressions in Kotlin with semicolons. So the question is: how does Kotlin infer where a statement or expression ends? Let's try to trick the compiler:

### Causing a CompilationException (wrong code generated)

Let's see what happens when we try to split up a simple calculation onto two lines:

```kotlin runnable
fun test() {
    return 2 + 
        3
}
```

