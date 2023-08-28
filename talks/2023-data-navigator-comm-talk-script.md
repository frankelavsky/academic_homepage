This is a default button. I'm sure you've all encountered them in various interfaces.

Of course, buttons can be clicked with a mouse or tapped with your finger. That's their default behavior.

But did you that most all buttons also allow you to "click" them using a keyboard? You can tab to them and press them using enter or spacebar.

And did you know that buttons will announce themselves as literal "buttons" when accessed by a screen reader?

This is how these elements work by default. And this is actually pretty accessible for people with disabilities.

These defaults are what I call "out of the box" accessibility or "downstream" accessibility. Someone made the buttons that UI designers and developers end up using. The people using them just automatically get value from someone else's work. Accessibility is easier to implement, there are less failures when people use these core elements, and now designers and developers have more time to focus on other, more interesting things than how a button should work with various assistive technologies.

But what about data visualizations?

This is a bar chart visualization. I can hover using a mouse to see a tooltip. With some charts I can even click the bars in order to do something like open some data or filter or go to a webpage.

This kinda sounds like button behavior, at least with my mouse.

But data visualizations often only have mouse support. Sometimes limited touch support.

So if someone wants to make a data visualization accessible, they have to figure out how to make charts and graphs navigable by screen readers, interactive with the keyboard, and work with other interaction modalities like voice commands and more.

Visualizations don't have good downstream accessibility.

In my chapter in Centering Accessibility in Data Visualization with the Urban Institute last December, I show that every charting library treats accessibility differently and most do almost nothing at all.

This is a problem because these libraries are now creating downstream *inaccessibility*.

And in my recent article published this summer in the Nightingale, the Journal for the Data Visualization Society, I explain that the burden generally falls to whoever is making the charts, not the tools, to fix access barriers. And I stress to my fellow data visualization practitioners that the fault of inaccessibility isn't entirely theirs.

I believe, and it is a core motivation in my work, that the responsibility of accessible visualization should first be carried by the toolkit makers and builders.

So in my latest project we built data navigator to help toolkit makers fix their ecosystems. Data Navigator provides an entirely new substrate, a layer of accessibility that interfaces with a broad range of input modalities, that can help toolkit makers continue to make great data visualization tools while also providing accessibility benefits for their downstream developers.

-----

Related work making data visualizations more accessible has recently begun to ramp up.

We have a breadth of research that explore what blind and low vision folks, primarily screen reader users, want from data visualizations and data experiences. Most data visualization literature focuses on vision-related disabilities.

When engaging blind and low vision folks in a digital context, the most common approach is to provide alternative text for a graphic. But unfortunately data visualizations complicate the simplicity of this approach.

This is a message my advisor sent me about a figure he was trying to write alt text for as he was preparing another paper. He said, "We need better tools. How do I even write an alt text for this figure that is reasonable?"

And research has demonstrated that you really cannot.

Traditional empirical work shows that providing simple alt text coupled with a data table that is formatted correctly is much better than just alt text.

But other research has also shown for years that tables increase cognitive load of users.

I'd argue that we visualize data to get away from tables. Our brains have a hard time seeing the forest when we look at one tree at a time. And of course, the approach of "" (shneiderman's drilling down thing and wickam's) is a cornerstone part of interacting with visualizations.

So the latest work to come out engaging this space is where I think things really start to get interesting.

In 2016 we had a paper by Sorge et al come out where they were engaging a structural problem. Alt text wasn't good enough and tables weren't good enough. In chemistry, the spatial relationships of different atoms in a molecule matter. And a table doesn't deal with this well.

They created a navigable visual, this works for both keyboards and screen readers.

Highcharts, a common charting library on the web, implemented this for their library of charts. In my prior industry work we also followed this pattern. We used up, down, left, right, and a drill in and drill out pattern.

And then Zong et all came along and provided deep co-design and empirical validation that this approach is actually really helpful for many visualization types, not just ones with a structural or spatial relationship, but even those we would traditionally only build tables for. They came up with an approach where a single visualization could be explored across multiple spatial and categorical dimensions (with a drill down approach) as well as with traditional tabular data.

I love this paper and it was a cornerstone for another piece that came out at CHI this year, Chart Reader, where they also explored ways to organize a rich, structural system for screen reader experiences of visualizations.

I believe that these papers have shifted the focus from making the visualization graphic itself accessible to making the spatial and structural relationships within that visualization accessible.

And I believe that for users of assistive technologies, this is a shift into thinking about the navigation of data and information.

But challenges remain for toolkit builders in the context of accessible data navigation. And until we address these challenges, we will continue to see downstream accessibility issues.

So, we frame our work around the goal of building a toolkit to help people who build visualization toolkits. A toolkit for toolkit makers.

The first and most fundamental challenge in modern visualization toolkits is that of structure.

Most visualization tools don't add an accessible, navigable structure at all. Those that do often reduce a chart to a list of data points, a table, or in the case of Olli, a hierarchy of lists within lists that also contain tables.

But these methods are not sufficient for all types of visualizations.

Some visualizations contain a structure that is geospatial, like a map. Using lists, tables, or hierarchies don't work.
(show and explain map)

Or a graph, with nodes and edges. A graph structure is a fundamentally different structure than a list, table, or hierarchy. Any node could have many, none, or a single connection to others, making navigation using existing structures impossible.

And of course there are mathematical diagrams, which might visualize a function. These display entirely spatial relationships, like 2 vectors with a vector sum or a set diagram (which is a venn).

And lastly are navigation structures that are actually made to tell a story through the data, where some spatial features or relationships are especially important in relationship to others and should be navigated in a particular order.

None of these structures which are important for accessibility are adequately addressed in visualization toolkits.

The second challenge for toolkits is that of input handling. Data visualization has been wrought with interaction troubles since touch devices rose in popularity. Predominantly still only mouse-driven (direct pointer) input is handled.

Remember that button example I opened with? Well data visualizations attempt to reinvent the button any time they build a chart. And assistive technologies are almost always excluded from interaction.

This also becomes a problem when building a navigable structure. Using something called ARIA, which are properties added to elements to make them accessible to screen readers, only helps screen readers. A native button works with a keyboard and a screen reader, but ARIA only helps one type of assistive technology.

And in HCI and accessibility contexts writ large, many, many other input modalities exist besides a mouse or screen reader.

In particular, the entirety of data visualization as a field, and in research contexts, has yet to reckon with how to make interactive visualizations accessible to users with motor and dexterity disabilities.

The input technologies used by these folks might be like a head-mounted pointer, which operates like a mouse. These folks are likely to face less barriers with interactive visualizations.

However users whose input technology relies on a keyboard, voice, gesture, or fabricated interface will likely face far more barriers.

These input technologies rely on either serial or direct navigation but their technologies don't benefit from ARIA in the same way that screen readers do.

And the last challenge is about rendering and semantics. This is related to how toolkits create data visualizations. Visualizations are generally rendered without semantics, as a raster image (like a png) or as SVG, a scalable vector graphic.

Semantics, or meaningful textual information, are added later.

Raster images, of course, are just pixels. Raster formats are the oldest and fastest ways of rendering. These two reasons are likely why this is still the most dominant type of visualization rendering.

Of course, the only way to make a raster image accessible is to add alt text to it. And then we run into those structural problems from before.

So SVG has become a popular rendering format, not only because the structure of rendered elements are stored as textual data, but also because ARIA can be added to that textual structure to make screen readers capable of navigating them.

However with SVG we run into the structural problem again: SVG and ARIA reduces all structure that might be in a visualization into a single list.

(explain vega lite)

And if that SVG is interactive, such that elements can be clicked or hovered in some way, only screen readers have access.

Going back to my opening example of a button:

If a data visualization had bars you could click, you'd actually want that to semantically be a button.

This is what the code looks like for a button. It says button! All kinds of nice technology works behind the scenes to make this button accessible to voice, keyboard, and screen reader devices out of the box.

This is an SVG element that is made to work like a button. It does not work with keyboard or voice input devices, only a screen reader. It's more work for toolkit makers and users and is less effective than something with out of the box accessibility.

So I now present our system design for data navigator:

Our system design was implemented on the web, in JavaScript, and uses HTML. However, our design is implementation agnostic and can be reconstructed in another environment as well, such as python, R, or even swiftUI.

We organized our design goals for the system into three separately composable subsystems, Structure, Input, and Rendering.

Toolkits all have different architectures, so it may be important to have distinct control over how each of these subsystems interact with each other and the toolkit architecture.

Each of these subsystems can be used in tandem with the others or separately, depending on their implementation.

So Structure.

We set out to create a new interface substrate, a new infrastructure, for building accessible interfaces. Most interface infrastructures are hierarchical. This, I believe, is why existing solutions for accessible visualizations can easily create list and hierarchy structures.

But our substrate instead is built on a graph structure. A graph is a structure formed out of nodes and edges. And nodes and edges can, of course, be used to represent virtually any other data structure: they can create tables, lists, and hierarchies. But they also can be used to represent network graphs, infographic and mathematical diagrams, flows, spatial structures like maps, and even custom paths through a visualization's story.

Nodes can be virtually anything, structurally. They can represent individual data points, groups of data points, or even information that isn't originally part of a dataset but could be encoded separately, like a title, axis label, visual feature, or annotation.

All navigation is facilitated by relationships. Navigation is about movement from somewhere to somewhere else. The relationships between nodes, which are edges, are how navigation, and navigation rules, are established. 

So a node contains a list of edges. Say, this one has 4. 

Each edge has information about the nodes it connects as well as a reference to which navigation rules can be called on that edge.

For example, this edge can move right when moving from our center node to this other node. And this edge would move left.

Navigation rules are what help introduce the second part of our system, which is Input.

Input is a system that handles events. So when Input is given a structure, it can process user input events across that structure. That means that say, a user is on this node again. And they are using a keyboard and press the right arrow key. The input system searches for the present node, looks at every edge, and finds which edge contains a navigation rules that matches the abstract rule for "right."

Navigation rules are highly flexible and are ideally declared in natural language. They represent a direction or location, such as "right" or "legend" and are what our input handler looks for when deciding how to turn user input into a navigation event.

And this pattern of input abstraction is actually borrowed from how the web handles what are called "pointer events."

A pointer click is an event that is detected as either a mouse click or a touch tap on a precise location.

Our system expands on this idea to use abstract movement that can then be invoked by virtually any possible input device.

Some examples:

A keyboard, naturally. The most important input to be able to handle.

Of course a screen reader works as well.

And then we can do more interesting things now that data visualizations haven't yet considered.

For example, I can interact with a chart on a small mobile device and I don't have to precisely click an element. I can actually swipe through a chart space the same way a mobile screen reader would swipe. The precise location of my finger is not as important as the movement and gestures I accomplish.

And while this isn't necessarily practical, of course this also works for any pointer device: here I just use a mouse to swipe as well.

Any input that can be validated into a command can be used with our system.

So here I've used a gesture recognition model to recognize that I am pointing as well as a few other hand gestures. I can navigate into the chart and around using gestures. This opens up many possibilities for future work.

And lastly, we demonstrate that even fabricated input devices work as well. Fabricated interfaces are a subject of study in accessibility contexts such as physical therapy, rehabilitation, working with children with disabilities, and the elderly. One particular study from 2017 used objects that could be found in a kitchen, primarily produce, to create a tangible interface for an aging community setting.

We validate our system works even with fabricated, produce-based interfaces.

And lastly, our final subsystem is rendering.

With this system I am actually expanding on my previous industry work. At Visa, I developed a pattern which we patented, where we would lazy-load an HTML-based accessibility structure over an existing SVG structure.

Our rendering subsystem now works whether or not the underlying structure is an SVG at all. And in addition, any HTML elements can be used. Our previous system only used images or buttons.

But this rendering system was improved and generalized on so that toolkit developers can continue rendering their visualizations in whichever way is best and still get robust out of the box accessibility that comes with well-designed elements like an HTML button.

For example, the charting library Highcharts, which I have written about many times as arguably the most robustly accessible charting library currently available, only provides their robust accessibility if a developer renders their charts using SVG.

And this is in conflict with canvas based rendering, which they demonstrate is far faster and more efficient than SVG to render.

Fast rendering matters. It has a smaller carbon footprint, better for users with low bandwidth, and provides a faster, more seamless interactive user experience.

Now with data navigator, libraries like highcharts can even make their canvas charts accessible.

I sent an early version of our system design, code, and paper to Moseng, the director of accessibility for highsoft, and he was ecstatic. They intend to build their own version of the data navigator internally.

So we have 3 demonstrations of our system that we show int he paper. I will only briefly discuss the last two since most of the system can be demonstrated with the first example.

This is a raster image of a barchart from highcharts. Here in the element inspector on the web we can see it is just a png image.

But now, I'll navigate into it with my keyboard. I can go across the title, axes, and now into the x axis. I'm moving across each stack here.

Keep in mind that the data used to render this chart doesn't include a datapoint for this stack. This is a computed group that appears when rendereding in this way. But data navigator has made this stack into it's own node in our structure. We even added tooltips. I can move left and right across this x axis dimension.

And I can go into the children and navigate left and right across the same x axis dimension again. But we also have this other dimension, and I can navigate up and down here as well. And each child node has multiple parents, so it isn't a true hierarchy. But instead we're demonstrating how a node-edge structure can be more useful.

So from a child I could press backspace. Now I'm back at the x axis groups. Again takes us all the way to the x axis itself. We'll go back in here. Now I can press L.

This takes me to the second parent of this child element, the legend groups. L key calls the Legend command. I can move up and down between these categories that are shown in the legend just like up and down moved across legend categories at the childmost level.

Now, the cool thing about data navigator is I can mix input modalities. I'm here on this group but now I will go over here to this text input and just type "legend" (which is does the same thing as the L key). And here now I am at the legend.

Enter. Enter again.

Right. Right. and so on.

One of my favorite parts about Data Navigator is a little feature I added where edges could actually have dynamic source or target assignments. An example of a dynamic source would be if I type Exit right now.

The dynamic source here is the same as "any node I am currently on" and the target is the exit element outside of the structure.

A dynamic source and target is an undo command. Any node can call it as a source and it could potentially call any other node.

Here let's navigate back in. 

I'll go into the legend and then undo. Now I am back at the legend. I'll undo again and now I'm back inside the legend.

This can also be used to navigate backwards through a history or whatever.

And why did I add this feature? Largely just to make the system more efficient. This way, one edge can be assigned to many nodes. It's just less memory compared to creating a specific edge for every node relationship.

Plus, visuals could change or animate or some actions, like undo or backwards through a history, are complex and can't be known at the time of instantiating our structure. Those can only be known after the user starts to interact.

So our second demonstration isn't a bespoke system like our first demo. In the first demo I wrote the code for the entire structure and traced the image to get a good looking visual focus indicator (that's the outline that appears on each element or group).

But the second demonstration is for our toolkit builders. In this demo I wrote some functions that can programmatically build a navigable structure, input handler, and renderer for almost any vega lite chart. It took me a relatively short amount of time and now a vega lite chart can also be rendered using webgl canvas, as more performant, but still get an accessibility experience equivalent to rendering with SVG.

Here it is really quick. We will use a screen reader this time. The root alt text is still there. That's part of vega lite when you render to canvas.

Entering in, navigating across the axes and now we are on a group of all the marks. Normally in SVG vega lite forces you to navigate some 400 points before you can move beyond this chart. Actualy torture for a screen reader user. So I simply created a single node to group these under. We could optionally enter into these here. We could explore around if we want. But we can also jump out and move on.

So the part that I'm sure toolkit developers will be excited about is our lazy-loading performance. We did several benchmark tests on vega-lite charts with different sized datasets. With a small dataset of 406 points (this original chart) Data Navigator increased initalization by a total of 5.25 milliseconds. When the dataset was 20,300 points the initialization time increased to about 10 milliseconds. This is almost negligable. If we render Vega lite using SVG the 20 thousand point chart takes 1,800 milliseconds. 5.25 extra is imperceptible. When rendering with canvas, the chart takes about 700 milliseconds, so an extra 10 is also imperceptible.

In our last demonstration example, our blind co-author and co-designer Lucas Nadolskis and I designed schemas for navigating vector and set diagrams. We wanted to demonstrate what it might look like to iterate on an unexplored navigation design space using Data Navigator. What spatial relationships matter? Which pieces should be navigable? How would we describe each part?

So what are our limitations and future work?

Well, we believe that our technical contribution opens up many lines of human studies and design work. We are presenting a system design, toolkit, and infrastructure for accessible data navigation. But more work should be done with users of assistive technologies to assess the system and establish ideal patterns for use.

Our most immediate future work is towards practical aims: we intend to improve the system, work to integrate it into existing toolkits alongside ttoolkit authors, and provide a user interface for building navigation structures by hand, without use of code at all. We believe that a well designed UI could open up our intended users from toolkit authors to anyone who wishes to make navigable graphics, not just data visualizations.
























