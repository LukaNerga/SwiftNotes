# 100 Days of SwiftUI

# Day 7 

## Creating Functions

```swift
func printTable(num: Int, end: Int) {
    for i in 1...end {
        print("\(i) * \(num) is \(i * num)")
    }
}
```

Calling the function:

```swift
printTable(num: 5, end: 15)
```

Functions let us reuse code.

---

## Returning Values

```swift
func rollDice() -> Int {
    Int.random(in: 1...6)
}
```

`-> Int` means the function returns an integer.

Single-line functions can omit the `return` keyword.

---

## Returning Multiple Values with Tuples

```swift
func getUser() -> (first: String, second: String) {
    (first: "Luka", second: "Gela")
}
```

Using the function:

```swift
let user = getUser()

print("Name: \(user.first) \(user.second)")
```

---

## Destructuring Tuples

```swift
let (first, second) = getUser()
```

Now each value is stored separately.

---

## Why Use Tuples?

Tuples are useful when a function needs to return multiple values.

You can access tuple values:
- by name
- or by index

Example:

```swift
func getUser() -> (String, String) {
    ("Luka", "Gela")
}

let user = getUser()

print(user.0)
print(user.1)
```

---

## External and Internal Parameter Names

```swift
func greet(_ name: String) {
    print("Hello \(name)")
}
```

`_` removes the external parameter label.

Calling:

```swift
greet("Luka")
```

---

## Parameter Labels

```swift
func square(of number: Int) {
    print(number * number)
}
```

Calling:

```swift
square(of: 5)
```

- `of` → external parameter name
- `number` → internal parameter name
- `Int` → parameter type
