---
sidebar_position: 2
---

# Border

Set your container border with rapid

## How to apply a border

Borders are applied using the following utility patttern `border` or `border-[range]`. You can remove the border with `border-0`


Here is an example

```dart
RapidContainer(
  styles: "border", // border with 1px width
  child: MyWidget()
);

RapidContainer(
  styles: "border-2", // border with 2px width
  child: MyWidget()
);

RapidContainer(
  styles: "border-0", // no border
  child: MyWidget()
);
```

## Accepted border symbols

* `border` which sets border to 1px width 
* `border-2` which sets border to 2px width 
* `border-4` which sets border to 4px width 
* `border-8` which sets border to 8px width 
* `border-0` which removes the border
