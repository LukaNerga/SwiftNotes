# 100 Days of SwiftUI

# Day 1 — Swift Basics

## Creating Variables

```swift
var greeting = "Hello Playground"
```

`var` creates a variable:

```swift
var name = "Luka"
```

`let` creates a constant:

```swift
let age = 20
```

Constants cannot be changed after creation.

---

## Using Quotes Inside Strings

To use quotation marks inside a string, use escape characters:

```swift
let quote = "He said \"Hello\""
```

---

## Multi-line Strings

```swift
let text = """
This is
multi-line
text
"""
```

---

## Useful String Methods

```swift
print(name.count)
```

Returns the length of the string.

### Uppercase Text

```swift
name.uppercased()
```

### Check Prefix

```swift
name.hasPrefix("Mr")
```

### Check Suffix

```swift
name.hasSuffix(".jpg")
```

---

## Readable Numbers

Large numbers can use underscores for readability:

```swift
let number = 100_000_000
```

Swift ignores the underscores.

---

## Checking Multiples

```swift
number.isMultiple(of: 3)
```

Checks whether a number is divisible by another number.

---

## Integers and Doubles

```swift
let a = 1       // Int
let b = 2.0     // Double
```

Swift does not allow adding different data types directly:

```swift
let c = a + b // Error
```

### Correct Conversion

```swift
let c = a + Int(b)
```

or

```swift
let c = Double(a) + b
```

---

## Type Safety

Once a variable is assigned a data type, it cannot later become another type.

```swift
var name = "Luka"
```

`name` will always store strings unless explicitly changed.
