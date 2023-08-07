---
sidebar_position: 3
---

# Border color

Set your border color with rapid

## How to apply a background color

Border colors are applied using the following utility patttern `border-[color]-[shade]`. Shades are in the range of 50-900 (in tailwindcss manner)

Here is an example

```dart
RapidContainer(
  styles: "border-grey-900",
  child: MyWidget()
);
```

## Accepted border colors

### No variant

* `border-white`
* `border-black`
* `border-transparent`

### With variants

* `border-amber`
* `border-blue`
* `border-blackgrey`
* `border-brown`
* `border-cyan`
* `border-deeporange`
* `border-deeppurple`
* `border-green`
* `border-grey`
* `border-indigo`
* `border-lightblue`
* `border-lightgreen`
* `border-lime`
* `border-orange`
* `border-pink`
* `border-purple`
* `border-red`
* `border-teal`
* `border-yellow`

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
  styles: "border-pink-50", // here 50 is the range of the color
  child: MyWidget()
);
```

