---
sidebar_position: 1
---

# Background

Set your container background with rapid

## How to apply a background color

Backgrounds are applied using the following utility patttern `bg-[color]-[shade]`. Shades are in the range of 50-900 (in tailwindcss manner)

Here is an example

```dart
RapidContainer(
  styles: "bg-grey-900",
  child: MyWidget()
);
```

## Accepted background colors

### No variant

* `bg-white`
* `bg-black`
* `bg-transparent`

### With variants

* `bg-amber`
* `bg-blue`
* `bg-blackgrey`
* `bg-brown`
* `bg-cyan`
* `bg-deeporange`
* `bg-deeppurple`
* `bg-green`
* `bg-grey`
* `bg-indigo`
* `bg-lightblue`
* `bg-lightgreen`
* `bg-lime`
* `bg-orange`
* `bg-pink`
* `bg-purple`
* `bg-red`
* `bg-teal`
* `bg-yellow`

### Variant color ranges
* `50`
* `100`
* `200`
* `300`
* `400`
* `500`
* `600`
* `700`
* `800`
* `900`

#### How to apply range to variant color

Here is a quick example

```dart
RapidContainer(
  styles: "bg-pink-50", // here 50 is the range of the color
  child: MyWidget()
);
```

