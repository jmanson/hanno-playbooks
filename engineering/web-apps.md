# Web apps

_We build complete full-stack web apps and services._

We usually build web or mobile apps with one of two frameworks, [Angular](https://angular.io/) or [React](https://facebook.github.io/react/).

From our POV, both are battle-tested enough to last in a production environment for a while (at least the next 5 years).

_Choosing between Angular and React is like choosing between buying an off-the-shelf computer and building your own with off-the-shelf parts._

_Angular 2 continues to put “JS” into HTML. React puts “HTML” into JS. HTML and JavaScript need to be glued together somehow, and React’s JavaScript-centric approach is fundamentally superior to Angular, Ember, and Knockout’s HTML-centric approach._

Here’s a brief comparison between the two, highlighting the pro and cons of each framework:

## React

* Is a library: you typically pull a number of other libraries off the shelf to build a real app
* It’s just the View Layer, which makes it a lot slimmer
* You write HTML in JS using JSX
* It is Javascript-centric
* It doesn’t exactly line up 1:1 with HTML tags
* For state management we’d use [Redux](http://redux.js.org/) (for most large apps) or [MobX](https://github.com/mobxjs/mobx) (for less complex apps that don’t need transactional state).
* For stuff that’s not baked in, you rely a lot on community-supported plugins

## Angular 2

* Is a framework: provides significantly more opinions and functionality out of the box
* It has significantly more boilerplate
* It’s HTML-centric
* It depends on TypeScript
* It relies a lot on dependency injection
* Has core support for forms, validation etc…
* Delivers performance gains with Ahead Of Time compiling (AOT) and tree-shaking
* Templates are an enhanced form of HTML, but you need to learn Angular DSL
