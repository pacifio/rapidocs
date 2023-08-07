---
sidebar_position: 4
---

# Axis size

Configure row/column size with rapid

## How to set axis size

To apply axis size you need to use the following pattern `axis-[min/max]`

Here is an example

```dart
RapidFlow(
  styles: "row justify-around axis-max", // this will take maximum horizontal space
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);

RapidFlow(
  styles: "column justify-center items-center axis-min", // this will take minimum vertical spacee
  children: [
    MyWidget1(),
    MyWidget2(),
  ],
);
```

## Accepted flow type symbols

* `axis-min`
* `axis-max`
