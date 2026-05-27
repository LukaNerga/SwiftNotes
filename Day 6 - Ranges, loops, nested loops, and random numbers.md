# 100 Days of SwiftUI

# Day 6 — Loops

## Ranges

### Closed Range

```swift
1...5
```

Includes both numbers:

```swift
1, 2, 3, 4, 5
```

---

### Half-Open Range

```swift
1..<5
```

Excludes the last number:

```swift
1, 2, 3, 4
```

---

## For Loops

```swift
for i in 1...12 {
    print("\(i)")
}
```

Runs the loop for every value in the range.

---

## Random Numbers

```swift
Int.random(in: 1...10)
```

Generates a random integer between 1 and 10.

---

## Nested Loops

A loop inside another loop is called a nested loop.

```swift
for i in 1...3 {
    for j in 1...3 {
        print("\(i) x \(j)")
    }
}
```

---

## Continue and Break

### Continue

```swift
continue
```

Skips the current iteration and moves to the next one.

---

### Break

```swift
break
```

Stops the loop immediately.

---

## While Loops

```swift
var countdown = 10

while countdown > 0 {
    print("\(countdown)")
    countdown -= 1
}

print("Done")
```

A `while` loop runs as long as the condition remains true.

---

## Practical Example

Finding the first 10 numbers divisible by both 4 and 14.

```swift
let num1 = 4
let num2 = 14

var multiples = [Int]()

for i in 1...100_000 {
    if i.isMultiple(of: num1) && i.isMultiple(of: num2) {
        multiples.append(i)

        if multiples.count == 10 {
            break
        }
    }
}
```

### Concepts Used

- loops
- conditions
- arrays
- `.isMultiple(of:)`
- `break`
