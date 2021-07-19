> SASS port of Chota

<p align="center">
<img src="https://jenil.github.io/chota/logo.svg" />
<br><br>
A really small (S)CSS framework
<br><br>
<img src="https://img.shields.io/npm/v/chotas.svg" alt="">
<a href="https://www.npmjs.com/package/chotas"><img src="https://img.shields.io/npm/dt/chotas.svg"></a>
<a href="https://github.com/Chaostheorie/chota/issues"><img src="https://img.shields.io/github/issues/Chaostheorie/chota.svg"></a>
</p>

<br>

-   ⚡️&nbsp; Super light-weight. Just ~3kb (minified + gzipped).
-   📐&nbsp; Magical 12 column [grid](https://jenil.github.io/chota/#grid) (can be customized)
-   🌈&nbsp; Easy to [extend](https://jenil.github.io/chota/#customizing) with SCSS maps
-   🎲&nbsp; Comes with a handful of [components](https://jenil.github.io/chota/#components) &amp; [utilities](https://jenil.github.io/chota/#utilities)
-   ✅&nbsp; Good Semantics
-   🤡&nbsp; Supports icons from [Icongram](https://icongr.am/)

<br>

### Get started

npm or yarn:

```bash
npm install chotas
```

```bash
yarn add chotas
```

#### SASS support

This SASS port of chota is designed for easy theming with SASS maps. This allows this port to be marginally smaller since it relies on colors directly and doesn't need to use the extensive CSS variable syntax.

To use the default color scheme:

```scss
@import '~chotas';
```

Use with custom maps:

```scss
@use 'sass:map';
@import 'chotas/sass/variables';

// Create your own color map
$custom-color-map: (
    // custom primary color
    'primary': #404147
);

// create your own layout map
$custom-layout-map: (
    // change to 4 col system
    'grid-cols': 4
);

// Merge the maps
$color-map: map.merge($color-map, $custom-color-map);
$layout-map: map.merge($layout-map, $custom-layout-map);

@import 'chotas/sass/utilities';
```

<br>

## Browsers support

| <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/edge.png" alt="IE / Edge" width="16px" height="16px" /></br>IE / Edge | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/firefox.png" alt="Firefox" width="16px" height="16px" /></br>Firefox | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/chrome.png" alt="Chrome" width="16px" height="16px" /></br>Chrome | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/safari.png" alt="Safari" width="16px" height="16px" /></br>Safari | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/opera.png" alt="Opera" width="16px" height="16px" /></br>Opera | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/safari-ios.png" alt="iOS Safari" width="16px" height="16px" /></br>iOS Safari | <img src="https://raw.githubusercontent.com/godban/browsers-support-badges/master/src/images/chrome-android.png" alt="Chrome for Android" width="16px" height="16px" /></br>Chrome for Android |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Edge 16+                                                                                                                                                           | last 2 versions                                                                                                                                                   | last 2 versions                                                                                                                                                | last 2 versions                                                                                                                                                | last 2 versions                                                                                                                                             | last 2 versions                                                                                                                                                            | last 2 versions                                                                                                                                                                                |

---

## Contributing

Welcome! Please see our [contributing guidelines](https://github.com/jenil/chota/blob/master/.github/CONTRIBUTING.md).

## License

SASS Port:

&copy; Cobalt 2021-present. Code released under the [MIT license](https://github.com/Chaostheorie/chota/blob/master/LICENSE_SASS).

Derived from Chota:

&copy; Jenil Gogari 2017-present. Code released under the [MIT license](https://github.com/jenil/chota/blob/master/LICENSE).
