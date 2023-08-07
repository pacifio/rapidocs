---
sidebar_position: 1
slug: /
---

# What is Rapid

Flutter rapid ui is a library that allows you to build responsive widgets quickly like tailwindcss. Rapid allows flutter developers to create responsive sharable widgets in record time with utility first tailwind like classes.

In rapid we call these classes utility symbols

<img alt="Rapid banner" src="/img/banner.jpg" />

## Why rapid

Making responsive widgets in flutter is a time consuming task, you have to wrap your widget in `LayoutBuilder` and calculate `maxWidth` and render different UI for different sizes of screens. But rapid allows you to do all of this with a single responsive prefix.

Here's a simple demo without the use of rapid

```dart
LayoutBuilder(builder: (context, constrains) {
  return Container(
    decoration: BoxDecoration(
      color: constrains.maxWidth > 600 ? Colors.green : Colors.red,
      borderRadius: BorderRadius.circular(12.0),
    ),
    padding: const EdgeInsets.all(12.0),
    margin: const EdgeInsets.all(12.0),
    child: const Text("Hello world"),
  );
});
```

And here's the same widget but with rapid

```dart
const RapidContainer(
  styles: "bg-green tab:bg-red px-3 py-3 mx-3 my-3 rounded-xl",
  child: Text("Hello world"),
);
```

## Install

Add rapid to your pubspec.yaml file like this

```yaml
dependencies:
  flutter:
    sdk: flutter
  rapid: ^0.0.1
```

## Rapid widgets

Rapid exposes 3 widgets as of version `0.0.1`

* `RapidContainer` a wrapper around the traditional flutter Container widget
* `RapidText` a wrapper around the traditional flutter Text widget
* `RapidFlow` a wrapper around the traditional flutter Row/Column widget

## Rapid demo

You can make truly responsive widgets in record time with rapid

```dart
import 'package:flutter/material.dart';
import 'package:rapid/rapid.dart';

class DemoCard extends StatelessWidget {
  const DemoCard({super.key});

  @override
  Widget build(BuildContext context) {
    return const Center(
      child: RapidContainer(
        styles:
            "px-4 py-4 mx-8 my-8 bg-grey-900 rounded-lg shadow-sm laptop:px-0 laptop:py-0",
        child: RapidFlow(
          styles: "column items-center axis-min laptop:row desktop:row",
          children: [
            RapidContainer(
              styles:
                  "w-16 h-16 laptop:w-32 laptop:h-40 rounded-full desktop:rect bg-grey-800 laptop:rounded-md",
              child: SizedBox(),
            ),
            SizedBox(
              height: 16,
            ),
            RapidContainer(
                styles: "laptop:px-8",
                child: RapidFlow(
                  styles:
                      "column items-center axis-min laptop:items-start desktop:items-start",
                  children: [
                    RapidContainer(
                      styles: "laptop:w-96",
                      child: RapidText(
                        text:
                            "Rapid allows flutter developers to create responsive sharable widgets in record time with utility first tailwind like classes",
                        styles:
                            "text-center text-white text-md laptop:text-left laptop:leading-relaxed",
                      ),
                    ),
                    RapidContainer(
                      styles: "pt-4",
                      child: RapidText(
                        text: "Adib Mohsin",
                        styles: "text-blue",
                      ),
                    ),
                    RapidContainer(
                      styles: "pt-1",
                      child: RapidText(
                        text: "layopay",
                        styles: "text-grey-500 uppercase text-xs",
                      ),
                    )
                  ],
                )),
          ],
        ),
      ),
    );
  }
}

```

## Rapid demo - Result

<video autoPlay muted loop style={{
  maxWidth: "100%"
}}>
  <source src="/demo/demo.mov"/>
</video>