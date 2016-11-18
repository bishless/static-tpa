# static-tpa

This is a static HTML version of the WordPress site (using a child theme for Justin Tadlock's excellent  [Stargazer](https://github.com/justintadlock/stargazer)) that resided at thirdpartyadministrator.net. When it came time to move it to a new host, it was clear that the site content hadn't been modified in a couple years. Meanwhile, the site was the target of numerous brute force login attempts and other attacks. Plus, it was a collection of < 20 unchanging pages w/ no blog posts of any sort.

I decided to convert it all to static HTML/CSS.

## Making Changes

The site is built from [CodeKit](https://codekitapp.com/)'s [.kit](https://codekitapp.com/help/kit/) extension of HTML. This was chosen for its offer of variables and partials.

CodeKit will build the site w/ little effort but it is not required. There are several compilers available for node, grunt, gulp, etc. (See [.kit compilers](https://npms.io/search?q=codekit))

### So much CSS

- [ ] Remove reliance on Stargazer/Dart #someday

### Those SVGs

_For future me that forgets how/why the SVGs are used the way they are on this build..._

SVGs from Illustrator or Sketch get optimized by CodeKit into the `/dist` directory. I then manually copy that optimized SVG code into new `_svg-<filename>.kit` partials to `@import` into other .kit files. Somewhat tedious, but seems to work well for reusing them across different pages/partials.

## Form Processing

I tried a few free form processors (el Formo, Formspree) and Brisk Forms won out. Quick and easy.
