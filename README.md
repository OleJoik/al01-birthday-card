# Android Codelab: Birthday greeting app
[Docs](https://developer.android.com/codelabs/basic-android-kotlin-compose-text-composables?continue=https%3A%2F%2Fdeveloper.android.com%2Fcourses%2Fpathways%2Fandroid-basics-compose-unit-1-pathway-3%23codelab-https%3A%2F%2Fdeveloper.android.com%2Fcodelabs%2Fbasic-android-kotlin-compose-text-composables#0)

# Packages
## AndroidX (Android Extension)
- Set of libraries and classes containing core functionality for app development
- Examples of imports used:
  - androidx.compose.material.Text
  - androidx.compose.ui.unit.sp

# Composables

## Text 

```
Text(
    text = "Some text"
)
```

Element can be styled using optional function arguments, such as `fontSize`.


## Trailing lambdas

Some composable functions, such as `Row` and `Column`, takes a lambda function `content` as their last parameter.

The following two chunks of code are identical in kotlin

```kotlin
Row(
    content = {
        Text("Some text")
        Text("Some more text")
        Text("Last text")
    }
)
```

```kotlin
Row {
  Text("Some text")
  Text("Some more text")
  Text("Last text")
}
```