---
sidebar_position: 2
---

# Justify

Configure main axis behaviour to row/column with justification symbols

## How to apply justify

To apply flow justify you need to use the following pattern `justify-[range]`

Here is an example

```dart
RapidFlow(
  styles: "row justify-around", // this will create a horizontal layout and spread widgets around
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);

RapidFlow(
  styles: "column justify-center", // this will create a vertical layout and group widgets together
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);
```

## Accepted flow type symbols

* `justify-center`
* `justify-start`
* `justify-end`
* `justify-between`
* `justify-around`
* `justify-evenly`
