# Static site generators

_Read which ones do we use and why_

We believe that in the majority of cases with a marketing website, the application’s backend logic can be handled once, at build time, to generate a static site. Any extra ‘dynamic’ functionality can be layered on with JavaScript.

Rather than building and maintaining a server, [Netlify](https://www.netlify.com/) and [Zeit Now](https://zeit.co/now) allow us to deploy a static site and simple build process with a few clicks and set this to run on every push to a master branch on GitHub. We can then relax knowing that the site we’ve deployed will be almost infinitely scalable and lightning fast. Other services are popping up more and more frequently.

That scenario is more common than you would think, and many Wordpress sites could probably be built this way, preventing Hackers from attacking the vulnerable PHP code it exposes (ever wondered why you need to update Wordpress every few days?)

Our favourite SSGs are:

* [Middleman](https://middlemanapp.com/): a Ruby-based tool that we have battle-tested in a lot of projects, including our own website.
* [Gatsby](https://github.com/gatsbyjs/gatsby): the new kid on the block. This tool allows you to write your static sites in React, and provides ultra-fast page-loading thanks to the React Router integration
* [Metalsmith](http://www.metalsmith.io/): another node.js-based tool that we’ve used and thanks to its strong plugin system allows for a very flexible and lean way of building static sites. Metalsmith powers this _Playbooks_ website.
