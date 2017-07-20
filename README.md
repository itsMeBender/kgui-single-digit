[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/itsMeBender/kgui-single-digit)

# Manipulating a single and multiple digits.

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
<kgui-multi-digits></kgui-multi-digits>
```

# Introduction

Manipulate a single or multiple digits, with mouse or keyboard. 
But mainly mouse, because keyboard usage, will overlay the keyboard on the app, hiding too much info.
This will be handy for small corrections of a number, like an INR value or dosing pills.

## Localization of decimal mark

The presentation of a number can be subject of localization, expecially when it concerns the __DECIMAL MARK__. A [decimal mark](https://en.wikipedia.org/wiki/Decimal_mark) is presented by a __DOT__ or __COMMA__ and is the divider of the fractional part of a number. The `kgui-multi-digit`-element `number` attribute supports both.

> _But, only the LOCAL presentation is used, in the number feedback_.

This means, that the value of _element.getAttribute('number')_ is localized. Containing a __COMMA__ for some European countries. And __DOT__ for other international standards, like JavaScript. You can use the _element.\_number_ property, to access the __JavaScript Number value__.

There is no automatic support for the thousand divider. Officially it is a _SPACE_. But using the __format__ attribute, you are free to use you own divider. For example '##-###-##'.

# Specifications

* Single digit manipulation.
* Multiple digits manipulation, using `<kgui-multi-digits number="123">`.
* Localization of the decimal-mark.
* Allow large number formatting, using (thousand) dividers.
* Number format also defines maximum size of the number. As in the format `###`, with number range from 0 .. 999.
* Currently only positive numbers are supported!

See also wiki.
