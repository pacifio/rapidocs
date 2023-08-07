---
sidebar_position: 8
---

# Text transforms

Manipulate text directly using rapid without calling dart string methods

## How to transform text cases

Here is an example

```dart
RapidText(
  text: "Demo",
  styles: "uppercase", // will result in DEMO
);

RapidText(
  text: "demo",
  styles: "capitalize", // Demo
);
```

## Accepted text transforms

* `uppercase`
* `lowercase`
* `capitalize`
* `normal-case`