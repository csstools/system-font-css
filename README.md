# System Font CSS

System Font CSS is set of `@font-face` rules that let you use the native system font of the OS running the browser.

```css
body {
    font-family: system-ui;
}
```

[system-font.css](system-font.css) offers eight variations of the `system-ui` font family; **light** (300) **light italic**, **normal** (400), **normal italic**, **medium** (500), **medium italic**, **bold** (700), and **bold italic**.

```css
blockquote {
    font: italic 300 system-ui;
}

p {
    font: 400 system-ui;
}
```

## Quick Start

### Install

This package can be installed with:

* [npm](https://www.npmjs.com/package/system-font-css): `npm install --save system-font-css`

### Load

When installed with npm, system-font.css will create both a SCSS and LESS partial for easy importing:

```scss
@import 'system-font';
```

## OSX

**OSX** has used three system typefaces. Since **El Capitan** it has used **San Fransisco**. In **Yosemite** it used **Helvetica Neue**. From **Mavericks** back to **Kodiak** it used **Lucida Grande**.

## Windows

**Windows** has used four system typefaces. Since **Vista** it has used **Segoe UI**. In XP, it used **Tahoma**, which oddly enough does not have an italic variation. From **Windows ME** back to **Windows 3.1** it used **Microsoft Sans Serif**. Finally, from **Windows 2.0** back to **Windows 1.0** it used **Fixedsys**. Neither **Microsoft Sans Serif** or **Fixedsys** are included in this set, with apologies.

Also, for those of opposed to joy, remember that **Internet Explorer 8** does not support local `@font-face` rules. Therefore, should you need to reference system fonts in that browser then you will need to do so from the `font` declaration.

```css
body {
    font-family: system-ui, "Segoe UI", Tahoma;
}
```

## Android

**Android** has used two system typefaces. Since **Ice Cream Sandwich** it has used **Roboto**. From **Jelly Bean** back to **Cupcake** it used **Droid Sans**, which also lacks an italic variation. Do you suppose OS developers dislike *emphasis*?

## Ubuntu

Ubuntu has always used one system typeface, aptly named **Ubuntu**. That part was easy.

## Native `system-ui` resources

* [CSS Fonts Module Level 4 Editor’s Draft Specification](https://drafts.csswg.org/css-fonts-4/#system-ui-def)
* [Chrome Platform Status](https://www.chromestatus.com/feature/5640395337760768)
* Proposed for inclusion on [Can I Use](https://github.com/Fyrd/caniuse/issues/2918)
* Previous [discussions in the W3C](https://lists.w3.org/Archives/Public/www-style/2015Jul/0169.html) to standardize a generic `system` family.
