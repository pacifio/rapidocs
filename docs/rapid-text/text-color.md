---
sidebar_position: 1
---

# Text color

Set your text color with rapid

## How to apply a text color

Backgrounds are applied using the following utility patttern `text-[color]-[shade]`. Shades are in the range of 50-900 (in tailwindcss manner)

Here is an example

```dart
RapidText(
  text: "Demo",
  styles: "text-green-900",
);
```

## Accepted text colors

### No variant

* `text-white`
* `text-black`
* `text-transparent`

### With variants

* `text-amber`
* `text-blue`
* `text-blackgrey`
* `text-brown`
* `text-cyan`
* `text-deeporange`
* `text-deeppurple`
* `text-green`
* `text-grey`
* `text-indigo`
* `text-lightblue`
* `text-lightgreen`
* `text-lime`
* `text-orange`
* `text-pink`
* `text-purple`
* `text-red`
* `text-teal`
* `text-yellow`

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
RapidText(
  text: "Demo",
  styles: "text-blue-50", // here 50 is the range of the color
);
```

