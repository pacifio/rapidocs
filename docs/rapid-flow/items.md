---
sidebar_position: 3
---

# Items

Configure cross axis behaviour to row/column with items symbols

## How to apply justify

To apply flow items you need to use the following pattern `items-[range]`

Here is an example

```dart
RapidFlow(
  styles: "row items-center", // this will create a horizontal layout and set crossaxis alignment to center
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);

RapidFlow(
  styles: "column items-start", // this will create a vertical layout and set crossaxis alignemnt to start
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);

RapidFlow(
  styles: "row items-baseline", // this will create a vertical layout and set crossaxis alignemnt to text baseline
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);
```

## Accepted flow type symbols

* `items-start`
* `items-end`
* `items-center`
* `items-baseline`
* `items-stretch`
