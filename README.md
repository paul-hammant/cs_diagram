# Client Side Diagram

Goals:

1. 100% ABI needed for "vertically align top edge of shapes to topmost of the edges of the selected shapes"
2. Clicking the v-align button should pop an overlay that has a sandboxed iFrame that deals with the ABI via https://github.com/Wizehive/post-rpc or one of the eight or so alternates

Constraints:  

1. All statically hosted - no server components for now. No persistence of the shape alignments needed.
2. In here we walk a skeleton.  Thin vertical slices and all that.
3. Small/Medium/Large tests after POC.
4. Tests needed to show nascent v-aligner can't bust out of iFrame (is contained), and would be too for multiple alternate JavaScript techs - Vue, Ng, React, Olde-Worlde JQuery.

