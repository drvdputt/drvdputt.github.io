# My "Github Pages" website

This website should be automatically built as long has the following is set up:
- The name of this repository needs to be exactly username.github.io
- The github pages setting needs to be enabled. Click the ‘Settings’ button on
  the repository home page. Then scroll down to the bottom where you see ‘GitHub
  Pages’ section and choose the master branch for the source.

I recently change the template to HTML5up "minimaxing". Edits to index.html
should be straightforward, since it's well documented with comments. The
website's mechanics are all in assets/css/main.css. Index.html references many
definitions from this file. So if I ever want to change the design of the
website, I should replace both the assets and the index.html structure by
something from a new template. After that, I should copy-paste everything from
the old website into the right places of index.html.

## Notes on CSS system

### Bootstrap grid (rows and columns)

A 12 column system. See main.css to see what a variet of things do with respect to this grid.

row -> container for the various column classes

col-(number 1 to 12): columns of varying widths, e.g. col-1, col-2

off-(number 1 to 12): offset by this much

Ideally, all the columns and offsets add up to 12. 

E.g.

```html
<div class="col-3 off-1">
    <p>narrow content</p>
</div>
<div class="col-8">
    <p>broader content </p>
</div>
```
