What is Archetype?
=====================
Archetype is my attempt at a flexible front-end framework for developers to get shit done quickly.

Using lessons learned from other popular frameworks (Bootstrap, Foundation et al), Archetype is meant to provide developers with all of the boilerplate that is part of the average front-end build but with a more flexible approach to customisation.

I'll expand upon this as I invest more time and effort into the project.

Building
=====================
I won't go in to massive detail here, as this is aimed at developers I will work on the presumption that you are capable of installing the required tools (or at least be able to google it).

The tools required for a successful build are as follows:

* Ant
* The Sass Gem
* CSSLint (I use the one from npm)
* YUI Compressor (Linked in your path as 'yuicompressor' - homebrew is your friend if you are on a Mac.)
* Some kind of JRE (Prerequisite of the above anyway)

I have bundled a jar of JSLint4java in the build directory as I am not 100% certain that the node version can output reports in a format my jenkins instance can understand, I will sort this later.

The ant build config is written with jenkins in mind, and outputs reports to build/logs should you wish to chuck this stuff through CI.

Building is simples, run `ant build` from the root of the project and you will get nicely built and compressed css and js in the respective directories of build/out.

Credits/Thanks
================
Archetype is copyright (C) 2012 Nick Pack.

With thanks to:
TwigKit (Semantic.gs) for the Awesome grid system.
Nicolas Gallagher and Jonathan Neal for Normalize.css

Licence
==========
Archetype is licensed under the Apache Licence 2.0, you can find a copy of this in the repository.

