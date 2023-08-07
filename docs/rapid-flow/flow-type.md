---
sidebar_position: 1
---

# Flow type

Rapid flow type sets the multiple children layout

## How to apply flow type

To apply flow type you need to use one of the following symbols, `row` or `column`

Here is an example

```dart
RapidFlow(
  styles: "row", // this will create a horizontal layout
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);

RapidFlow(
  styles: "column", // this will create a vertical layout
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);
```

## Accepted flow type symbols

* `row`
* `column`
