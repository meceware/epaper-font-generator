# ePaper Font Generator

This little Python tool can convert `ttf` fonts to `sFont` file needed for ePaper displays.

PS: This tool is not tested much but works on my machine :) Please open a pull request (desired) or let me know an error.

## How to use

This tool analyzes the given font and draws and finds the best possible width for the font to display.

If `width` parameter is given, this is used instead of analyzed width value.

```python
py .\main.py --font .\font\Helvetica-Monospaced-W06-Rg.ttf --height 64 --margin-vertical 1 --margin-horizontal 1
```

## How it works

Basially, the script draws text over image and analyzes the best possible results. The best possible font size is analyzed to make sure the font is fit inside the given width/height value. Afterwards, the text is centered in the image right before the `sFont` is generated.

## License

MIT