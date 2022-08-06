# Client Side Diagramming

Preview: [https://paul-hammant.github.io/cs_diagram/](https://paul-hammant.github.io/cs_diagram/)

Goals:

1. 100% ABI needed for "change fill color"
2. Clicking the 'color' button should pop an overlay that has a sandboxed iFrame that deals with the ABI via https://github.com/Wizehive/post-rpc or one of the eight or so alternates

Constraints:  

1. All served from SAME ORIGIN, yet **constrained** via iframe sandboxes,
1. All statically hosted - no server components **for now**. No persistence of the shape alignments needed.
2. In here we walk a skeleton.  Thin vertical slices and all that.
3. Small/Medium/Large tests after POC.
4. Tests needed to show nascent fill-color-changer can't bust out of iFrame (is contained), and would be too for multiple alternate JavaScript techs - Vue, Ng, React, Olde-Worlde JQuery.

