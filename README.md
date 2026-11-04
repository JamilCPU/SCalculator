# SCalculator

A JavaFX calculator that was meant to evaluate typed arithmetic expressions (for example `3 + 4 * 2`) using the four basic operations and standard order of operations. The window with an input box and a Calculate button is in place, but the evaluation logic is unfinished.

## Stack

- Java with JavaFX (no build tool; plain source files)

## Running

There is no Maven or Gradle file, so compile and run with a JavaFX SDK on the module path. Replace `<path-to-javafx-sdk>` with the location of your JavaFX SDK.

```
javac --module-path <path-to-javafx-sdk>/lib --add-modules javafx.controls *.java
java  --module-path <path-to-javafx-sdk>/lib --add-modules javafx.controls Window
```

Tokens in the expression must be separated by spaces.

## Project layout

- `Window.java` - JavaFX window with the expression box, Calculate button and result field
- `Arithmetic.java` - tokenising and operator-precedence evaluation

## Status

Work in progress and not functional: the expression evaluator is incomplete (for example, the add, subtract and divide helpers still contain multiplication logic, and tokens are not converted to numbers). It was abandoned in that state.
