[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/itsMeBender/kgui-single-digit)

# Manipulating a single, multiple digits.

<!---
```
<kgui-single-digit>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="kgui-single-digit.html">
    <next-code-block></next-code-block>
  </template>
</kgui-single-digit>
```
-->
```html
<kgui-single-digit></kgui-single-digit>
```

# Introduction

Manipulate a single digit, with mouse or keyboard. 
But mainly mouse, because keyboard usage, will overlay the keyboard on the app, hiding too much info.
This will be handy for small corrections of a number, like an INR value or dosing pills.

It is part of a construction where multiple singe digits interacts and can modify a large number.

# Specifications

* Single digit manipulation.
* Localization of the decimal-mark.
* Multiple digits manipulation, using `\<kgui-multi-digits\>.`
* Allow large number formatting, using dividers.
* Number format also defines maximum size of the number. As in the format `###`, with number range from 0 .. 999.

## Future enhancements

* Decimals (I'm working on this (july'17).
* Negative numbers.
