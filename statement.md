# Breaking Kotlin



## Breaking the Compiler

As you know, you don't normally need to end all statements and expressions in Kotlin with semicolons. So the question is: how does Kotlin infer where a statement or expression ends? Let's try to trick the compiler:

### Causing a CompilationException (wrong code generated)

Let's see what happens when we try to split up a simple calculation onto two lines:

```kotlin runnable
fun main(args: Array<String>) {
    val a = 42
    
    when (a) {
        in Math.abs(-1)..100 -> println("It's between 1 and 100")
    }
}
```

