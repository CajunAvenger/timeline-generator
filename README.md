# timeline-generator
 An HTML/CSS tool for generating timelines.
 
A Timeline is made of one or more Threads. A Thread is a collection of Events which are displayed sequentially in the Timeline. Multiple threads at once is supported.

The management panel is split into four tabs, Timeline, Threads, Events, and Export.

## Timeline
The Timeline tabs has controls for the global settings for the entire graph.

* Boundary Dates: Sets the edges of the display. Events may exceed the boundaries, but will only be rendered within them.
* Major axis: Controls the size of the major axis markers.
* Axis style: Controls how major axis marers are displayed.
* Date labels: Controls the label pattern for the major axis. The relevant year, month, or date is input as {Y}, {M}, or {D}.
* Timeline height: Controls the height of the timeline render. Has a minimum sized based on Major Axis.
* Bar width: Controls the width of event bars.
* Milestone width: Controls the widths of "milestone" events, those with a 0 time duration.
* Label width: Controls the width of the event bar labels.
* Label offset: Controls the spacing between the thread's bar and its event labels.
* Thread offset: Controls the spacing between threads.
* Axis offset: Controls the horizontal placement of the axis bar.
* Axis label offset: Controls the vertical placement of the axis labels.
* Bar offset: Controls the spacing between the axis and the first thread.

## Threads
* Thread selector: Controls thread being edited.
* New thread: Create a new thread at the end of the timeline.
* Current thread name: The display name of this thread, editable.
* Current thread index: The display index of this thread, editable.
* Current thread color: The default color for this thread's events, editable.
* Bar width offset: Adjusts the bar width for this thread's events.
* Label width offset: Adjusts the label width for this thread's events.
* Label offset: Adjusts the bar/label spacing for this thread's events.
* Thread offset: Adjusts the spacing between this thread and the next one.
* Delete thread: Deletes the thread and all its events.
* Merge threadd: Deletes the thread and moves its events to another.

## Events
* Events are created with a start date, end date, and optionally a label and color.
* Clicking on an event brings up its edit menu, which allows editing any of the above as well as adding:
* Label offset X, Y: Fine tune the label placement for the event.
* Change thread: Change which thread this event is attached to, or create a new thread containing just this event.
* Delete event: Remove the event entirely.

## Export
* Import timeline: Allows importing an existing timeline to start from there.
* Export files: Exports several files for displaying the timeline elsewhere:
 * timeline-import.txt, for importing in the previous command.
 * stylesheet.txt, for the CSS code for the final timeline.
 * stylesheet-html.txt, for the HTML code that goes with it.
 * stylesheet.html, an HTML file of both of those.
 * inline-html.html, an HTML file where all styling is rendered with inline CSS rather than CSS rules.