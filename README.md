My TechRadar
============

This is not a "manifesto" - I'm looking to write down my idea of "optimal"
web stack, alongside the rationale. Something that puts all the
parts together may not exist yet, and I'm looking to evolve this piece
as I go. Name is a shameless rip-off of "ThoughtWorks Tech Radar"

TypeScript
----------

I have developer a strong preference for selecting TypeScript over
CoffeeScript, plain Javascript or ES6 transpilers. This is the easiest
choice in this list.

CONS:

- Larger initial investment due to smallel community (tools,
  build scripts, learning)

PROS:

- Code is safer (less scary) to extend and modify, even in areas
  that have no unit tests (or that are hard to test)

- Static types and proper intellisense increase productivity, esp. with
  code you haven't written yourself

Angular.JS
----------

Angular has the overwhelmingly highest mindshare among MVC frameworks at
the moment. In absence of fatal flaws, community momentum alone makes
it a conservative choice.

Angular has been accused of being harder to learn than some of the
competition, but this is an upfront cost that is easily amortized
over the usage cycle. Once you know how to use it, it's a very productive
environment that helps Get Stuff Done with small amounts of code.

While competing MVC frameworks have areas where they may do better than
Angular, it's unclear whether they will gather big enough community
to be well maintained through years to come.

Comments on some competing frameworks in particular:

- Backbone: doesn't do much. You have to assemble lots of pieces (like test
  automation) to make the offering competitive with Angular.

- Ember.js: direct competitor to Angular, losing in mindshare rapidly


SASS
----

(Note: jury is still out on this one)

Seems to be the current "winner" in CSS preprocessors. Syntax (SCSS) is
compatible with CSS, so you can copy-paste snippets from the web,
and team members that don't need the advanced features can just write
normal CSS.

Main argument is more readable and configurable CSS, with little extra
cost / overhead. Compass is the main "mixin library" for SASS, but
brings complexity overhead that may not be worth the while. Personal
preference would be to deploy SASS without Compass.

Gulp
----

Gulp is simpler and apparently much faster than Grunt.

Gulp has less available plugins than Grunt, but quantity does not
necessarily imply quality here - some Grunt plugins just don't work properly,
and then you end up in complex debugging scenarios. Gulp seems to be
easier to debug: it's imperative rather than declarative, and tasks
are composed of finer granurarity "building blocks" whose behavior
you can probe without implementing full plugins yourself.

Gulp is much faster than Grunt, which can greatly improve productivity
in a long term project with several developers going through edit - save -
livereload cycle hundreds of times a day.

Judging by the "pulse", Gulp also seems to be preferred by the more
"advanced" audience. This is a good indicator on the direction
the industry is going.

Browserify
----------

To be written
