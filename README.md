# incanter-gorilla

[Gorilla REPL](http://gorilla-repl.org) integration for [Incanter](http://incanter.org).

## Usage

Add `[incanter-gorilla "0.1.0-SNAPSHOT"]` to your project as well as the lein-gorilla plugin (see
Gorilla REPL's [getting started](http://gorilla-repl.org/start.html) page for help with installing Gorilla).
You can then `(use 'incanter-gorilla.render)` in your Gorilla worksheets.

To display Incanter chart in your worksheet use `(chart-view pl)`, where `pl` is any JFreeChart generated
by Incanter. Note that a snapshot of the current state of the plot is shown in the worksheet so: dynamic
plots will not work; and you should add all annotations etc before viewing the plot (of course, you can
view it more than once!). The `chart-view` function takes `:plot-size` and `:aspect-ratio` options.

You can see an example Gorilla worksheet
[here](http://viewer.gorilla-repl.org/source=github&user=JonyEpsilon&repo=gorilla-test&path=ws/incanter.clj)
that shows some Incanter plots.

## License

This code is licensed to you under the MIT licence. See LICENCE.txt for details.

Copyright © 2014- Jony Hudson