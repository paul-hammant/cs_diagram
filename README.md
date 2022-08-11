# Client Side Diagramming

Preview: [https://paul-hammant.github.io/cs_diagram/](https://paul-hammant.github.io/cs_diagram/)

[The Principles of Containment](https://paulhammant.com/2016/12/14/principles-of-containment) applies.

# Goals

1. 100% ABI needed for secure operations. For now that's a one-line JQuery operations passed to eval(). JQuery is MIT license. If it were 1989, I'd say [ARexx](https://en.wikipedia.org/wiki/ARexx) was the best Inter-Process-Communication tech.

# Constraints

1. Toolbar buttosn should pop an overlay that has a sandboxed iFrame that deals via window.postMessage(..)
2. All served from SAME ORIGIN, yet **constrained** per #1
3. All statically hosted - no server components **for now**. No persistence of the shape alignments needed while testing the operations on the SVG canvas
2. For enhancements to this prototype, we walk a skeleton.  Thin vertical slices and all that.
3. Small/Medium/Large tests after POC.
4. Pen tests needed to show nascent fill-color-changer can't bust out of iFrame (is actually contained), and would be too for multiple alternate JavaScript techs - Vue, Ng, React, Olde-Worlde JQuery.

# Progress

There's two toolbar widgets:

* Fill (all) shapes with a color - via a color picker (see [JsColor](http://jscolor.com) - GPL)
* Change (all) shapes outer lines - either bigger or smaller than they are already - plain JavaScript.

Both of those have no dependencies.

The "server" side (the window with the SVG canvas) has 17 lines of JQuery-using JavaScript, that is mostly 
the communication between with the toolbar widgets in sandboxed iframes.