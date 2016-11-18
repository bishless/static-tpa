# static-tpa

This is a static HTML version of the WordPress site that resided at thirdpartyadministrator.net. When it came time to move it to a new host, it was clear that the site content hadn't been modified in a couple years. Meanwhile, the site was the target of numerous brute force login attempts and other attacks. Plus, it was a collection of < 20 unchanging pages w/ no blog posts of any sort.

I decided to convert it all to static HTML.

## Making Changes

The site is built from CodeKit's .kit extension of HTML. This was chosen for its offer of variables and partials.

CodeKit will build the site w/ little effort but it is not required. There are several compilers available for node, grunt, gulp, etc. (See [.kit compilers](https://npms.io/search?q=codekit))

## Form Processing

I tried a few free form processors (el Formo, Formspree) and Brisk Forms won out. Quick and easy.
