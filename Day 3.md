# 100 Days of SwiftUI

# Day 3 — Arrays, Dictionaries, Sets, Tuples, and Enums

## Arrays

Arrays store multiple values in order.

```swift
let names = ["Luka", "Nika", "Gio"]
```

Access values using indexes:

```swift
print(names[0])
```

⚠️ Accessing an index that does not exist will cause an error.

---

## Adding Items to Arrays

```swift
var numbers = [1, 2, 3]

numbers.append(4)
```

`.append()` adds a new item to the end of the array.

---

## Array Type Safety

Arrays can only store one type of data.

```swift
var scores = [10, 20, 30] // Int array
```

```swift
var names = ["Luka", "Nika"] // String array
```

---

## Empty Arrays

```swift
var numbers = Array<Int>()
```

or

```swift
var names = [String]()
```

---

## Useful Array Methods

### Count Items

```swift
names.count
```

### Remove Item at Index

```swift
names.remove(at: 2)
```

### Remove All Items

```swift
names.removeAll()
```

### Check if Item Exists

```swift
names.contains("Luka")
```

### Sort Array

```swift
names.sorted()
```

### Reverse Array

```swift
names.reversed()
```

---

## Dictionaries

Dictionaries store data as key-value pairs.

```swift
let student = [
    "name": "Luka",
    "major": "Computer Science"
]
```

Access values using keys:

```swift
print(student["name"])
```

---

## Default Values in Dictionaries

To avoid getting an optional value:

```swift
print(student["age", default: "Unknown"])
```

---

## Empty Dictionaries

```swift
var scores = [String: Int]()
```

Add values:

```swift
scores["Luka"] = 100
```

⚠️ Duplicate keys cannot exist.

---

## Sets

Sets store unique values.

```swift
let numbers = Set([1, 2, 3])
```

Sets:
- cannot contain duplicates
- have no fixed order

---

## Empty Set

```swift
var names = Set<String>()
```

### Insert Into Set

```swift
names.insert("Luka")
```

---

## Tuples

Tuples allow storing multiple values together.

```swift
let user = ("Luka", 20)
```

Access values:

```swift
print(user.0)
print(user.1)
```

---

## Enums

Enums define a group of related values.

```swift
enum Weekday {
    case monday, tuesday, wednesday, thursday, friday
}
```

Using enums:

```swift
var day = Weekday.monday
```

Changing values:

```swift
day = Weekday.friday
```

Swift can infer the enum type:

```swift
day = .friday
```
