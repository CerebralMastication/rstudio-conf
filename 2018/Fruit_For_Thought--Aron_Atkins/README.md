# Fruit for Thought

This directory contains the slides, speaker notes, and demo files from the
"Fruit for Thought" talk from rstudio::conf 2018 by [Aron
Atkins](https://github.com/aronatkins).

## Slides

The slides for the talk are in [`index.html`](index.html) with accompanying
speaker script in [`speaker.md`](speaker.md) (compiled to
[`speaker.html`](speaker.html) using custom CSS with `pandoc`).

```
pandoc -s -c speaker.css -o speaker.html speaker.md
```

## Demo R Markdown files

* [`demos/image.Rmd`](demos/image.Rmd) - very simple R Markdown file showing
  just the image
* [`demos/macoun.Rmd`](demos/macoun.Rmd) - complete R Markdown report
  restricted to Macoun apples
* [`demos/simple.Rmd`](demos/simple.Rmd) - first pass at adding report
  parameters
* [`demos/parameterized.Rmd`](demos/parameterized.Rmd) - complete
  parameterized report using selector, text, and slider input controls

## Datafiles

The [`demos/watercolors.json`](demos/watercolors.json) datafile comes from
https://github.com/thisisparker/datasets and had one record manually adjusted
(see: https://github.com/thisisparker/datasets/pull/1).

The [`demos/thumbs.json`](demos/thumbs.json) was generated by a modified
`pomfetch.py` from https://github.com/thisisparker/pomtiles (see:
https://github.com/thisisparker/pomtiles/pull/2). The demos during my talk
took advantage of locally-cached images to avoid any possible WiFi issues. The
Rmds in this directory have been updated to use wikimedia URLs instead.
