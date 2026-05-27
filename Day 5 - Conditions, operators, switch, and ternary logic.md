# 100 Days of SwiftUI

# Day 5 — Conditions and Switch Statements

## If Statements

```swift
if someCondition {
    print("Do something")
} else if conditionB {
    print("Do something else")
} else {
    print("Else")
}
```

`if` statements run code only when conditions are true.

---

## Comparison and Logical Operators

### AND Operator

```swift
&&
```

Both conditions must be true.

---

### OR Operator

```swift
||
```

At least one condition must be true.

---

### NOT Operator

```swift
!
```

Reverses a Boolean value.

---

### Equal To

```swift
==
```

Checks whether two values are equal.

Example:

```swift
if age == 18 {
    print("You are 18")
}
```

---

## Enums with Switch Statements

```swift
enum Weather {
    case sun, rain, wind, unknown
}
```

Create a value from the enum:

```swift
let forecast = Weather.sun
```

---

## Switch Statements

```swift
switch forecast {
case .sun:
    print("It's sunny")

case .rain:
    print("Take an umbrella")

default:
    print("Unknown weather")
}
```

`switch` checks multiple possible values.

---

## Fallthrough

```swift
fallthrough
```

Continues execution into the next case.

Example:

```swift
switch number {
case 1:
    print("One")
    fallthrough

case 2:
    print("Two")

default:
    break
}
```

---

## Break

```swift
break
```

Stops the switch or loop immediately.

---

## Ternary Conditional Operator

Short form of an `if` statement.

```swift
let age = 18

let canVote = age >= 18 ? "Yes" : "No"
```

Structure:

```swift
condition ? trueValue : falseValue
```
