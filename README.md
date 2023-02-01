<h1 align="center">Svelte Weather</h1>

<p align="center">
<a href="https://svelte-weather.codewithshin.com/">Svelte-Weather</a>
</p>

<p align="center">
<a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps"><img src="https://img.shields.io/badge/PWA-enabled-brightgreen" alt="PWA Shield"></a>
<a href="https://www.npmjs.com/package/svelte-weather" rel="nofollow"><img src="https://img.shields.io/npm/v/svelte-weather" alt="npm"></a>
<a href="https://twitter.com/shinokada" rel="nofollow"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow"><img src="https://img.shields.io/github/license/shinokada/svelte-weather" alt="License"></a>
<a href="https://www.npmjs.com/package/svelte-weather" rel="nofollow"><img src="https://img.shields.io/npm/dw/svelte-weather.svg" alt="npm"></a>
</p>

210+ SVG weather icons for Svelte. Svlete-Weather-Icons support major CSS framework. You can add additional CSS using the `class` props.

<p align="center">
<img width="650" src="/static/images/weather-optimized.png" />
</p>

## Installation

```sh
npm i svelte-weather
```

## Icon names

[Icon names](/icon-list.md)

## Icon images

[Icon images](/icon-images.md)

## REPL

- [Demo 1](https://svelte.dev/repl/d98438528d974bb7981357fa20e92137)
- [Demo 2](https://svelte.dev/repl/cf8a7f1be1f14d839d72784c4a377a65)

## Usage

```js
<script>import {DayCloudy} from "svelte-weather";</script>
```

## Props

| Name      | Default   |
| --------- | --------- |
| size      | 30        |
| class     |           |
| ariaLabel | file name |

## Size

Use the `size` prop to change the size of icons.

```html
<DayCloudy size="30" />
<DayCloudy size="40" />
<DayCloudy size="50" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<DayCloudy color="#ff0000" /> <DayCloudy color="#00ffd8" />
```

## CSS framework support

Use the `class` prop to change colors and add additional css.

For example, Tailwind CSS:

```html
<DayCloudy class="text-pink-700 mr-4" />
```

If you use the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<DayCloudy class="text-pink-700 dark:text-blue-300" />
```

Bootstrap example:

```html
<DayCloudy class="position-absolute top-0 px-1" />
```

## aria-label

All icons have aria-label. For example `DayCloudy` has `aria-label="day cloudy"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<DayCloudy ariaLabel="day cloudy icon" class="text-red-500"></DayCloudy>
```

## Passing down other attributes

You can pass other attibutes as well.

```html
<DayCloudy tabindex="0"></DayCloudy>
```

## Import all

Use `import * as Icon from 'svelte-weather`.

```html
<script>
  import * as Icon from 'svelte-weather';
</script>

<Icon.DayCloudy size="30" class="text-red-500" />
<Icon.DirectionRight size="40" class="text-blue-700" />
<Icon.Hail size="50" class="text-green-700" />
<Icon.MoonAltWaningGibbous2 size="60" class="text-purple-500" />
<Icon.NightAltSleet size="100" class="text-purple-500" tabindex="0" />
```

## Original source

[erikflowers/weather-icons](https://github.com/erikflowers/weather-icons)

## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)

## PWA: Fast & Offline

This website can be downloaded and installed on your device for offline access as a Progressive Web App.

To install a PWA, look for the "Add to Home Screen" option in the browser's menu or settings. On most mobile devices, this option can be found by visiting the website, then selecting the "Options" or "Menu" button in the browser, and looking for the "Add to Home Screen" option. On some desktop browsers, right-click on the page and select "Install".
