
# hypercat

> :link: + :octocat: =
  an SVG-based octocat-flavored hyperlink to your GitHub repository.

## Usage

To put a hypercat in a document, please follow these simple steps.

1. Copy the [`hypercat.svg`](hypercat.svg) file into your project.
2. Adapt the `href` value, and (maybe) the `title` one.

   ```svg
   <a xlink:href='https://github.com/<username>/<repository>'
     xlink:title='Check the source code on GitHub!'
     target='_top'>
     ...
   </a>
   ```

3. Add the following line into your HTML document, after the opening `<body>` tag.  
  (This is just one way—of a handful of different approaches—to embed an SVG file.  
   You can learn more in
   [this short tutorial](https://www.sitepoint.com/add-svg-to-web-page/)—or maybe,
   you’d rather read a somewhat [extended one](https://css-tricks.com/using-svg/).)

   ```html
   <object data='hypercat.svg' type='image/svg+xml'></object>
   ```

4. Finally, attach this CSS rule into your stylesheet.

   ```css
   object {
     position: absolute;
       top: 0px;
     right: 0px;
   }
   ```

## Design

This repository was inspired by
[Tim Holman’s approach](https://github.com/tholman/github-corners).  
I created a slightly different design, offering some round corners
and a colorful animation. :art:

## Credits

This little project was made possible with the help of

- [GitHub](https://github.com)’s octocat,
- the fresh and original design made by [@tholman](https://github.com/tholman),
- and [Inkscape](https://inkscape.org), the open-source vector graphics editor.
