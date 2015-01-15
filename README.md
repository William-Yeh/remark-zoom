remark-zoom
===

Zoom in/out facility for remark.


## Purpose

[remark](https://github.com/gnab/remark) is a simple, in-browser, markdown-driven slideshow tool targeted at people who know their way around HTML and CSS. It works well, but a strange issue bothers me that, browser's zoom in/out hotkeys are disabled by the remark (see [issues](https://github.com/gnab/remark/search?q=zoom&type=Issues&utf8=%E2%9C%93) at the remark project's repository).

**remark-zoom** tries to provide zoom in/out facility for remark.


## Usage

Load the `remark-zoom.js` script file *after* `remark-latest.min.js`.  For example,

```html
<!-- load remark.js main script -->
<script src="https://gnab.github.io/remark/downloads/remark-latest.min.js" type="text/javascript"></script>
<script>
    var slideshow = remark.create();
</script>

<!-- load our remark-zoom.js -->
<script src="remark-zoom.js" type="text/javascript"></script>
```


Feel free to link to the online version of `remark-zoom.js`, hosted at GitHub:

```html
<script src="https://raw.githubusercontent.com/William-Yeh/remark-zoom/master/remark-zoom.js" type="text/javascript"></script>
```

## Keystrokes

The **remark-zoom** accepts the following keystrokes while viewing slides:


- `+` (plus): zoom in.

- `-` (minus): zoom out.

- `0` (zero): reset to normal size.

When these keys are pressed, all texts will be zoomed immediately. *Images*, however, will be zoomed only when *mouse over*.


## Online demo

<a href="http://william-yeh.github.io/remark-zoom/">remark-zoom demo</a>, hosted at GitHub Pages.


## To view the slides locally

1. Change working directory to the slide directory.

2. Start a local web server, e.g.:

   ```
   $ python -m SimpleHTTPServer 8000
   ```

3. Use any modern web browser to view the slides:

   - Zoom demo: http://localhost:8000/demo.html

   - Remark intro (copied from [remarkjs.com](http://remarkjs.com)): http://localhost:8000/remark-intro.html



Feel free to change the port for HTTP.

Reference: https://github.com/gnab/remark/wiki#external-markdown




## Tested browsers

I have only tested the **remark-zoom** for the following browsers. Feel free to fork and create push requests.


OK:

  - Chrome (on Mac): 37.0.2062.124

  - Firefox (on Mac): 34.0


Zoom for image doesn't work:

  - Safari (on Mac): 8.0.2





## License

Licensed under Apache License, Version 2.0.

Copyright © 2015 William Yeh.
