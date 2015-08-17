# Changes 2.0

Development branch: TODO

Issues / Tickets: [Issues in a grid](http://code.google.com/p/piccolo2d/issues/list?can=1&q=label%3AMilestone-2.0&colspec=ID+Type+Status+Priority+Milestone+Owner+Toolkit+Component+Summary&x=owner&y=status&mode=grid&cells=tiles)

## Package structure

Goal: eliminiate circular (intra-jar) dependencies.

## Event Subsystem


## Property Change Handling

The Bubbling up of Property Changes uses bitwise comparison to determine if it should be dispatched up the hierarchy. Since the default is to not bubble up, this seems to be adding a whole lot of code to the core for something that's rarely used.

mro: Let's see how awt, swing, swt (and Cocoa touch) do it an pick the best ideas.