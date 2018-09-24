# Wireframe UI

Wireframe UI is a clone of Atom One Light UI but with an SVG pencil filter added for a black-and-white wireframe effect.

## Why?

The SVG filter Wireframe UI utilizes is actually part of the [Inkscape](https://inkscape.org/en/) filter bundle. That entire bundle of awesome filter effects is included in the /assets/ folder as filters.svg.

There are 2 benefits:
- easy access to all of Inkscape's scalable filter effects within Atom.
- dead simple starting point for building UI themes relying on Atom One Light UI.

In short, anyone can fork this repo to create their own UI theme with easy access to amazing SVG filters.

All credit goes to the Atom One Light UI and Inkscape teams for their great work.

### Settings

In the theme settings you can:

- Change the __Font Size__ to scale the whole UI up or down.
- Choose between 3 __Tab Sizing__ modes.
- Hide the  __dock buttons__.

To make changes, go to `Settings > Themes > Wireframe UI > Settings` or the cog icon next to the theme picker.

### Customize

It's also possible to resize only certain areas by adding the following to your `styles.less` (Use DevTools to find the right selectors):

```css
.theme-one-light-ui {
  .tab-bar { font-size: 18px; }
  .tree-view { font-size: 14px; }
  .status-bar { font-size: 12px; }
}
```

### FAQ

__Why do the colors change when I switch Syntax themes.__
This UI theme is based on Atom One UI theme which uses the background color from the chosen syntax theme. If that syntax theme has a dark background color, it only uses its hue, but otherwise stays light. This lets you use light-dark combos.
