---
sidebar_position: 2
slug: /prefix
---

# Responsive prefix

Make responsive widget with only a short few lines of utility symbols

## Accepted responsive prefix

There are only 4 responsive prefix

* `mobile` applied between 0-600px width of the device
* `tab` applied when device is greater than 600px
* `laptop` applied when device is greater than 1200px
* `desktop` applied when device is greater than 1400px

## How to apply a prefix

You can apply a prefix to any valid utility symbols, you need to use the following pattern to apply a responsive prefix `[prefix]:[valid-symbol]`

Here is a quick example

```dart
RapidContainer(
  styles: "laptop:w-96", // width set to 384 px if the device is a laptop and it is applied for bigger devices
  child: RapidText(
    text:
        "Rapid allows flutter developers to create responsive sharable widgets in record time with utility first tailwind like classes",
    styles:
        "text-center text-white text-md laptop:text-left laptop:leading-relaxed", // text alignment set to center for smaller devices and text alignment will switch to left for bigger devices, same case for text line height
  ),
);
```

