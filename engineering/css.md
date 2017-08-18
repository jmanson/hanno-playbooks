# CSS

_More about our CSS workflow and tools_

## Frameworks

To save time and money, we avoid building the HTML/CSS structure from scratch, and rely on pre-built framework solutions instead.

In the past, we’ve used both, [Foundation](http://foundation.zurb.com/) and [Bootstrap](http://getbootstrap.com/). Nowadays, we’re more inclined to use Foundation as most of us are more familiar with it, and we think it’s the more robust and advanced solution.

Since we do a lot of prototyping, building the basic HTML and CSS boilerplate usually feels like a huge waste of time. That’s why we usually start out by using a front-end UI framework to provide a responsive grid, some solid UI components and the usual JavaScript enhancements that you’d need in every project.

We then tweak the existing grid, default styles (like colors and margins/padding) and UI components to our needs. From our experience, there is no faster way than this to quickly prototype a new product idea and put it in the hand of our users.

It’s very rare that we’d write the entire CSS for an application from scratch, simply because of the huge technical and maintenance effort that this requires. It’s usually something we recommend against, since the baseline styles included in these CSS frameworks have been tested in the wild by millions of people and provide a decent experience on a huge number of platforms and devices.

That said, in a few cases we have taken on this task and are experienced with and open to use more minimal solutions such as [Pure CSS](https://purecss.io/) or something less opinionated and more flexible like [Susy](http://susy.oddbird.net/). In the end, it’s all about catering to the project’s requirements and setting up a speedy and streamlined development process.

## Our workflow

We make heavy use of [SASS](http://sass-lang.com/) for better organisation of styles, integrated into a solid build process (e.g. [Webpack](https://webpack.js.org/), [Grunt](https://gruntjs.com/) or [Middleman](https://middlemanapp.com/)). We highly recommend using preprocessors to increase readability and maintainability of your CSS.
