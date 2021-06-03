# ✅ Getting Started

To install UIToolkit-Styles on your project you can either install it with npm or from CDN.

## 🛠 Install:

Install the library from npm by running the following command on your project:

```bash
$ npm install @symphony/uitoolkit-styles --save
```

Or using yarn

```bash
$ yarn add @symphony/uitoolkit-styles
```

Import the main css file on your project:

```bash
 import '@symphony/uitoolkit-styles/dist/css/uitoolkit.css';
```

Using webpack will serve automatically font files

You can also import the SASS version:

```bash
  @import '~@symphony/uitoolkit-styles/uitoolkit.scss'
```

In some cases (depending on your bundling solution) you might need to indicate the icon fonts path changing the `$ICONS_FONTS_PATH` variable, with **myPath** pointing to the fonts directory under **node_modules/@symphony/uitoolkit-styles/dist/fonts**

```bash
 $ICONS_FONTS_PATH: 'myPath/fonts';
```

## 🔗 Link

To work locally with uitoolkit-styles, e.g. `yarn link`, please change the following value

path: `src/icons/_index.scss`

```bash
 $ICONS_FONTS_PATH: '../fonts' !default;
```

## 📦 Install from **CDN**:

Alternatively, you can use the [symphony](https://cdn.symphony.com/resources/ui-toolkit/master/css/uitoolkit.css) CDN to load the compiled CSS version.

Import the prefered css on your project:

```bash
<link rel="stylesheet" href="https://cdn.symphony.com/resources/ui-toolkit/v1.0.10/css/uitoolkit.css">
```

**Note**

For development purposes, if you want to test the latest features you can use the master version from the CDN:

```bash
<link rel="stylesheet" href="https://cdn.symphony.com/resources/ui-toolkit/master/css/uitoolkit.css">
```

## 📏 Sizing units

The UIToolkit Styles library bases all the Unit mesurements on the `rem` unit.

It is fixed to a base of `16px`. If you need to update it on your project you can change `$UITOOLKIT_REM_BASE` variable.

path: `src/utils/functions/_index.scss`

```css
$UITOOLKIT_REM_BASE: 14;
```

## 🧪 Sandbox

<iframe src="https://codesandbox.io/embed/serverless-wood-ty6t6?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="ui-toolkit-styles-sandbox"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>
