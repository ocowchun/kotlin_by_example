In Kotlin you can declare an identifier either through `var`(short for variable) or `val`(short for value)

`var` is reassignable while `val` is not.

When declaring a new identifier, consider using `val` first and change it to `var` only when reassignable is needed.

```kt
val valueList = mutableListOf<Int>()
var variableList = mutableListOf<Int>()
valueList.add(1)
variableList.add(2)
variableList = valueList
// valueList = variableList // Val cannot be reassigned
```
