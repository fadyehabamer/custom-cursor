# Custom Cursor
> Using  Css + Svg encoder

Hover over the image to see the mouse cursor replaced by a custom SVG crosshair. The SVG (`cursor.svg`) is URL-encoded with [yoksel's URL-encoder for SVG](https://yoksel.github.io/url-encoder/) and inlined in `style.css` as a `data:` URI:

```css
.custom-cursor {
    cursor: url("data:image/svg+xml,...") 25 25, pointer;
}
```

The two numbers are the hotspot (the exact click point, here the centre of the 50x50 image), and `pointer` is the fallback cursor.

**Live demo:** https://fadyehabamer.github.io/custom-cursor/

## Run locally

No build step. Open `index.html` in a browser.
