# 100 Days of SwiftUI

# Day 2 — Booleans and String Interpolation

## Booleans

Booleans store either `true` or `false`.

```swift
let isGood = true
let isBad = false
```

Booleans can also come from expressions:

```swift
let isMultiple = 120.isMultiple(of: 3)
```

---

## Toggling Booleans

```swift
var gameOver = false
gameOver.toggle()
```

`.toggle()` switches a Boolean value:

- `true` → `false`
- `false` → `true`

It is similar to using `!` (NOT operator).

---

## Joining Strings

```swift
let people = "Georgians"
let action = "hate"

let tradition = people + action + "Russians"
```

Usually it's cleaner to add spaces manually:

```swift
let tradition = people + " " + action + " Russians"
```

---

## String Interpolation

String interpolation inserts variables into strings using `\(variable)`.

```swift
print("People from Georgia are \(people)")
```

Example:

```swift
let age = 20

print("I am \(age) years old.")
```
