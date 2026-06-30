ALT TEXT FOR EVERY FIGURE
Source: main.tex

======================================================================

1. figures/figure 2.png
   Testing the contrast of a chart and fixing it.

2. figures/figure 3.png
   The navigation order is shown on a stacked bar chart, zig-zaging forward. It is then fixed to show multiple possible paths, left/right or up/down.

3. figures/figure 4.png
   Showing a mouse interacting with a stacked bar chart and updating a table.

4. figures/figure 5.png
   A chart with almost no text compared to a chart with a robust explanation.

5. figures/figure 6.png
   This section is about a screen reader (that's what you're using, I reckon, Hello!). The chart on the left is interactive but the screen reader semantics are uninformative. On the right, it states the role (toggle button) as well as gives feedback (selected).

6. figures/figure 7.png
   A chart that shows a trend next to a table that shows the month-by-month data for that trend listed out.

7. figures/figure 8.png
   A dense scatterplot being accessed one element at a time compared by a screen reader to a dense scatterplot where the main outlier cluster (the important part) is being accessed instead.

8. figures/figure 9.png
   A bar chart that has patterned textures combined with color changing into black and white (but still with textures).

9. data_navigator.png
   A diagram that shows an image of rich, accessible, navigation structures, icons for robust input handling, and additional graphics for flexible, semantic rendering. These images, icons, and graphics all feed into Data Navigator, which feeds into visualization toolkits, shown with a variety of different data visualization types (maps, scatterplots, lines, graphs, and bar charts).

10. figures/state-of-the-art.png
   4 different diagrams. 1. Raster image*: Start, image, end. The diagram is a straight line with 3 nodes. 2. SVG with ARIA*: Start, svg, mark 1, repeating pattern, mark n, end. Straight line with 5 nodes (and repetition). 3. Vega-Lite* (SVG+ARIA): Start, svg, x axis, y axis, mark 1, repeating pattern, mark n, legend, end. Same as SVG with ARIA but it has axes and a legend. 4. Olli**: This diagram has a main line with 7 nodes, 4 of which have branches off of them. Start, root, x axis, y axis, legend, grid, and end. The x axis shows intervals, a table, rows, and cells underneath. The y axis, legend and grid all have a note that their pattern is similar to the x axis.

11. figures/geoviz.png
   A map, tree, and graph representation. The map is encoded with colors according to engineers per capita. The tree shows a recursive pattern and a focus indicator, as if a user has navigated to Alabama then to neighboring state Florida. Instead of backing out of the structure, the user continued to navigate between them, which created a large amount of waste and repetition between these two states and their corresponding lists of neighboring states. The graph representation shows a start, Alabama, Alaska, Arizona, and a repeating symbol. Connected to Alabama are example neighboring nodes, each listed once: Mississippi, Tennessee, Georgia, and Florida.

12. figures/simple_movement.png
   A diagram with 4 parts: 1. Code. // using movement dn.move('right') 2. Two nodes, BPL-A and BPL-C, an arrow pointing from BPL-A to BPL-C. 3. Code. // an edge instance 'bpla-bplc': { source: 'bpla', target: 'bplc', navRules: ['right', ...] } 4. Code. // a navigation rule right: { key: 'ArrowRight', direction: 'target' }.

13. figures/dynamic_movement.png
   A diagram with 4 parts: 1. Code. // using movement dn.move('previous position') 2. Two nodes, any node and previous, an arrow pointing from any to previous. 3. Code. // a generic edge 'any-return': { source: (_d, current, _p)=> current, target: (_d, _c, previous)=> previous, navRules: ['previous position', ...] } 4. Code. // a navigation rule 'previous position': { key: 'Period', direction: 'target' }.

14. figures/inputs.png
   Image in two parts. First part: Inputs: A. Hand swiping. B: Speaking 'left.' C. A hand gesture on camera. D. Bananas. Second part: Output: (focus moves left) A focus indicator has moved on a bar chart from one stacked bar to another on its left.

15. figures/semantics.png
   A diagram showing the node Alabama connected to the node Counties which is connected to a table of counties. A return link has an arrow from the table back to the Alabama node. Next to the Alabama node is the code: semantics: { attributes: { role: 'image', id: 'alabama-node' }, description: 'Alabama. 0.004 Engineers per capita. Contains 67 counties.' } Next to the Counties node is the code: semantics: { element: 'a', attributes: { href: '#alabama-table' }, description: 'Alabama Counties Data Table.' }.

16. figures/path.png
   Code used to render a path that looks like an outline which then places that outline over visual elements on a data visualization. A. Node with path supplied. Code. bpl: { id: 'bpl', edges: [...], renderId: 'render-bpl' } render-bpl: { x: 194, y: 609, width: 918, height: 116, path: 'M987 136 H 985 L 985 137 L 848...', cssClass: 'dn-path', semantics: {...}, visualId: null } B. Path rendered, shown on an empty space. C. Path overlaid on visual space, over a data visualization. The path snugly wraps around a group of elements.

17. figures/static.png
   Large, 4 part diagram. (This diagram demonstrates why a single alt text isn't enough. Too bad PDFs can't have data navigator work inside of them.) A. Raster (png) visualization, showing a stacked bar chart 'Major trophies for some English teams' B. Dual tree schema design. A graph with a main line containing 6 nodes: Start, title, legend, y axis, x axis, end. The legend and x axis each branch off into axis items 1 through n and legend items 1 through n. Both of those trees rejoin on the same children elements, sub-bar 1 through sub-bar n. Arrows are shown that map between the sub bars, from the sub-bars up to the axis and legend items, and then up to the axis and legend nodes. C. Keyboard navigation rules. Rules show LEFT/RIGHT moves across axis items, UP/DOWN moves across legend items, PERIOD moves back to user's last location, ESCAPE exits the structure, ENTER moves in along either the axis or legend while BACKSPACE moves out towards the axis and L moves out towards the legend. D. Schema instantiated. The pattern from B is applied to the chart in A, so every single node is shown rather than a generic stand-in node like 'axis item' or 'sub bar,' such as 'Arsenal' and 'BPL-A.'

18. figures/vega-lite.png
   2 part figure. Part 1: A. Various Example Vega-Lite Charts. A line chart, bar chart, and scatter plot are shown in default styling. Part 2: Diagrams. B. Canvas. Start, image, end. C. SVG + ARIA. Start, svg, x axis, y axis, mark 1, repeating pattern, mark n, legend, end. D. Canvas + DN. The same diagram as C. E. Canvas + DN (improved). The same diagram as C except that mark 1 through n are nested under a mark group, so that the marks can be skipped without navigating through all of them.

19. figures/braille.png
   A. Reference parallel vector diagram, a color diagram showing 2 vectors and a vector sum plotted on an x y Cartesian space. B. Traced portion, a black and white diagram showing one vector, the vector sum, and the parallel of the second vector used to calculate half of the vector sum. C. Braille pin array output, an image of how a refreshable braille display shows the triangular shape of the traced portion.

20. figures/sets.png
   A. Reference, a color diagram of two sets that intersect. The sets are shown as perfect circles. B. Structure, a 6 part break down of the navigable structure. Each node is shown as a traced subportion used to render to the braille display. Walkthrough: 1 is both sets, 2 is the left set, 3 is the intersection of the two sets, 4 is the right set, 5 is the subset of the left set that is excluded from the right set, and 6 is the subset of the right set that is excluded from the left set.

21. figures/vectors.png
   A. Reference, a color diagram showing 2 vectors and a vector sum plotted on an x y Cartesian space. B. Structure, a 10 part breakdown of the navigable structure. Each node is shown as a traced subportion used to render to the braille display. 1 is the whole diagram, 2 is only vectors, underneath 2 are 3 traced portions, 1 for each vector. 3 is the whole diagram, underneath are the left and right halves of the equation used to calculate the sum, one for each vector and the opposite vector's parallel vector. Underneath each of these are the vectors and their own parallel vectors.

22. library_boundary.png
   A diagram divided by a dashed boundary line. On the right, "data-navigator, the npm library" contains three module boxes: dn.structure, which builds nodes, edges, dimensions, and navigation rules and can ingest Vega-Lite views; dn.input, a traversal engine with move, enter, exit, and key validation functions; and dn.rendering, a semantic HTML overlay with a wrapper, entry and exit elements, and one focusable node at a time. A gray strip below lists utilities and geometry helpers. On the left, three application-layer boxes connect across the boundary: structure design, which authors or generates nodes, edges, and rules, feeds dn.structure; modality adapters, which translate keyboard, swipe, gesture, speech, and text events into rule names, feed dn.input; and the host visualization with the focus lifecycle, which exchanges rendering calls with dn.rendering.

23. skeleton
   Skeleton's interface. There is a tree-like structure with 3 hierarchical levels shown in the schema. In the editor, outlines shown over the 3 lines in a line chart, along with vertical bands that join the lines at each month they cross. These two shapes appear like a triple helix. On the right is a panel labeled scaffold, which has options for setting various parameters.

24. figures/geologic.png
   A zoomed out view of the state of Wisconsin, encoded with a tapestry of dozens of colors and textures. Arrows annotate direction from the legend to map area, a separate area has messy, approximated graph structures laid out, a zoomed in version of a chart inside the graphic has schematics next to it titled "grid navigation." An area in the upper corner demonstrates 2 different styles of drawing tooltips during navigation.

25. figures/scaffold.png
   A scatterplot, stacked bar, and line chart. Each has a graph next to it that shows nodes and edges. On the other side of each chart is a version of itself with grides, outlines, and marks that represent the various shapes and locations that the nodes and edges take over the chart's space.

26. figures/label_preview.png
   Label builder UI. Show interface options, label template filled with generic pattern-building text, and then a label preview shows output "New York, trend for temp: flat, average temp: 13.78, City 3 of 8. Long description of UI details: title "Aggregate summaries from children" unselected count of children, unselected min and max of dropdown with temp selected, unselected sum of dropdown with temp selected, selected average of dropdown with temp selected. "Trend direction and r squared options" x variable dropdown with month selected, y variable dropdown with temp selected, selected trend direction, unselected r squared.

27. figures/skeleton_padding.png
   Four visualizations, a bar chart, scatter plot, stacked bar chart, and line chart. Each visualization is shown twice, first with outlines overlaid that are slightly offset and then again with the outlines almost perfectly overlaid on the elements they represent.

28. figures/voronoi_pie.png
   A voronoi pie chart with a large slice emphasized. A large text caption reads, Small assignments: 26 small assignments will make p 45% of your grade. These exercises, games, quizzes, activites, readings, critiques, and discussions are to be completed in-class on the same day they're issued. Showing up and being present will go a long way to earning you full credit.

29. hero
   A schematic of a device with a rail and two handles. This device manipulates a chart and a separate chart is rendered as a tactile graph on a refreshable braille display.

30. figures/proto.png
   Our prototype with a blown up version where all the parts are shown separately.

31. figures/schematic.png
   Wiring schematic of the cross-feelter. A Teensy 4.0 microcontroller connects over USB to a host computer running the browser app. Each of two motorized faders exposes six terminals: two track ends, a touch line, a wiper, and two motor terminals. The track ends of both faders are wired across the Teensy's 3.3 volt and ground pins. The wiper of fader 0 connects to analog pin A0 and its touch line to A1; the wiper of fader 1 connects to A2 and its touch line to A3. Teensy digital pins D2 and D3 drive the AIN1 and AIN2 inputs of a DRV8833 dual H-bridge motor driver for rail 0, and pins D4 and D5 drive the BIN1 and BIN2 inputs for rail 1; the driver's AOUT and BOUT pairs connect to the two fader motors. The driver's motor supply pin takes 5 volts from the Teensy's VUSB pad, so one USB cable powers the entire device. A note summarizes the serial protocol: the device reports both rails as JSON every 50 milliseconds, the host commands a rail with a rail id, a four-digit target, and a newline, and motor targets are cancelled while a knob is touched.

32. figures/analysis.png
   Our analytical environment with 3 visualizations as well as instructions for connecting devices and controlling the filter.

33. figures/quant.png
   A panel of nine small charts comparing two conditions for 15 blind participants: the cross-feelter and the screen reader alone labeled in a legend at the top left. Six of the charts are unit-column charts, where each small square is one participant; the other three (task time and the two data-query measures) are split density plots, with the cross-feelter distribution drawn on the left in blue and the screen reader distribution on the right in gray. Results are covered in more detail in the body of this chapter and the supplemental materials released on OSF for this paper draft.
   <!-- The nine charts:

   Completion rate (counts; 0 or 1). At "1" (task completed) the blue cross-feelter column is tall, covering nearly all participants, while the gray screen reader column is noticeably shorter. At "0" (not completed) blue is just a single square while gray has several. Cross-feelter mean 0.93 versus screen reader 0.60.

   Accuracy (correctness) (counts; 0 or 1). At "1" (correct answer) the blue column is slightly taller than gray, and at "0" (incorrect) blue is slightly shorter than gray. The gap is small. Cross-feelter mean 0.67 versus screen reader 0.53.

   Task time (in seconds) (split density, axis ~0 to 200+). The blue cross-feelter distribution bulges low on the axis, centered roughly between 50 and 100 seconds. The gray screen reader distribution sits higher and is roughly double-humped, with weight near 100 and again near 170 seconds. Cross-feelter mean ~76s versus screen reader ~144s — about 90% faster.
   
   Data queries (computational) (split density, axis ~0 to 30+). The blue distribution is large and stretches well up the axis, into the 20s and beyond, while the gray distribution is small and bunched near the bottom, roughly 0 to 10. Cross-feelter mean ~20 versus screen reader ~7.

   Data queries (spoken) (split density, axis ~0 to 15+). The blue distribution is the larger and more spread, reaching up toward 15, while the gray distribution is smaller and concentrated lower, around 5. Cross-feelter mean ~8 versus screen reader ~5.
   
   Anxiety (Likert 1 to 5, unit columns). This chart shows two measures at once: outlined, unfilled bars mark each participant's pre-task baseline anxiety (an arrow annotation labels these "Pre-task"), and solid bars mark anxiety about a future timed data task. The solid blue cross-feelter bars cluster low, mostly at 2 to 3, while the solid gray screen reader bars cluster higher, mostly at 3 to 5; the unfilled baseline bars are scattered across the middle and upper range for both. Cross-feelter future-task mean 2.27 versus screen reader 3.00 — and the cross-feelter's future anxiety fell below participants' own pre-task baseline, while the screen reader's did not.

   Stress (Likert 1 to 5, unit columns). The blue cross-feelter ratings pile up at 2, with a few at 3 and 4, while the gray screen reader ratings spread higher across 3, 4, and 5. Cross-feelter mean 2.40 (median 2) versus screen reader 3.20 (median 3).
   Cognitive load (Likert 1 to 5, unit columns). Both conditions peak at 3 and look similar overall, with blue and gray columns of comparable height at 3 and 4. Cross-feelter mean 3.13 versus screen reader 3.47 — comparable.

   Enjoyment (Likert 1 to 5, unit columns). The blue cross-feelter ratings cluster high, at 4 and 5, while the gray screen reader ratings cluster low, at 2 and 3 with a couple at 1. Cross-feelter mean 3.93 (median 4) versus screen reader 2.33 (median 2). -->

34. figures/future.png
   4 diagrams. 1. Using pre-rendered embossed graphics when a refreshable braille display is not available. A stack of embossed papers is being used with the feelter. 2. Utilizing both rails: one to navigate, one as output based on position. A line chart is shown with the 2-rail version of the feelter. 3. Using knobs, joysticks, and other tactile input that suit different data types. A knob is shown turning while a visual focus of the knob is shown over two complex circular visualizations. 4. Cross-feeltering, brushing, zooming, and panning in 2 or more dimensions. A scatterplot is shown being filtered with a square shape brush overlay. The overlay's 4 sides are controlled with 2 cross-feelters, one for each axis.

35. options.png
   A collection of 4 different configurations of the same dashboard.

36. dashboard.png
   A preferences menu is shown on the left, with an explanation of how to use, and a series of UI controls and toggles for options under the headings Comprehension, Text visuals, Color and contrast, Element size, and Audio. Each category has a collapsed subsection beneath the heading for showing more options. A dashboard sits next to the menu.