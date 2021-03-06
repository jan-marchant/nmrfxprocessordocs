---
title:  Mouse and Keyboard
taxonomy:
    category: docs
---

The mouse can be used in multiple modes.  The two primary modes are a Crosshair mode in which
crosshairs can be displayued and moved and a Selector mode in which items can be selected and regions can be "dragged out".

## Using the Crosshair Cursor

T> NMRFx can show two sets of crosshairs.  If you're using a 1-button mouse (or the trackpad on a laptop) the mouse moves the black crosshair at first.  The red crosshair will appear if you then click at some distance away from the black crosshair. Further actions of clicking and dragging will move whichever crosshair is closest when you click.  NMRFx will recognize that you have a 3-button mouse as soon as you click with either the second or third mouse button.  Once recognized, the black crosshair will be moved when the left mouse button is down, and the red crosshair when the middle mouse button is down.

**To display the crosshairs:**

Click the left mouse button with the pointer positioned at the location
you want the first crosshair line(s) to appear.

Click the left mouse button away from the black crosshairs, or click the middle mouse button anywhere, to get the second crosshairs (red).

**Status panel displays crosshair positions**

As the crosshair lines are moved around the spectrum the status panel is
continuously updated with their positions (in PPM). 


The crosshair positions can be precisely adjusted by typing a value into
the status panel entries for each of the crosshair lines. After entering
a value, hit the Return key to move the crosshair to the new position.
This is useful to, for example, set up exact expansions of the spectrum.

**To move an existing crosshair:**

Press and hold the left mouse button with the pointer near the first
crosshair. Keep the button down as you drag the crosshair to a new
position. If you first position the pointer near the intersection of two
crosshairs lines, then both crosshairs will move. If you position the
point near a single crosshair line (vertical or horizontal), then only
that crosshair will move. Use the middle mouse button to position the
second crosshair. Note: as described above, you can initially move
both crosshairs with the left mouse button.  Once you use the middle
button, the crosshairs are black and red crosshairs are moved
with the left and middle buttons respectively respectively.

You can switch between one-button (both crosshairs move with left
button) and two-button mouse modes with key bindings.  Type c1
to switch to one-button mouse mode and c3 to switch to two button
mouse mode ("c3" because this is typically used with three button
mice)..

**To remove the crosshairs:**

Click the redraw button in the control panel to the right of the
spectrum. When the spectrum is redrawn the crosshairs will not be
displayed.

**To move the spectrum region**

Hold down the Command key (Mac OS X) or Control key (Windows or Linux)
and click and drag with the left mouse button. The spectrum will pan
left and right along with the cursor. With 2D spectra you can also pan
the spectrum region vertically.

**Status panel displays crosshair positions**

As the crosshair lines are moved around the spectrum the status panel is
continuously updated with their positions (in PPM). The horizontal
distance (in Hz) between the two vertical crosshair lines is also
displayed. This can be useful for the manual measurement of couplings.
The crosshair positions can be precisely adjusted by typing a value into
the status panel entries for each of the crosshair lines. After entering
a value, hit the Return key to move the crosshair to the new position.
This is useful to, for example, set up expansions of the spectrum.

**Moving the crosshairs in multiple spectra (correlation)**

The crosshair in different windows automatically track each other in
what is generally an appropriate manner. No commands are required to
start correlated crosshair tracking. Crosshair correlation is dependent
on the label given to each axis of the spectrum during the referencing
process. For example, consider the case where 5 windows are open, with
axis labels as indicated below.

|Window-Name   |X-axis label   |Y-axis label  |
|------------- |-------------- |--------------|
|a             |15N            |1HN           |
|b             |13C            |15N           |
|c             |1H1            |1H2           |
|d             |1HN            |13C           |
|e             |15N            |1HN           |
|------------- |-------------- |--------------|

  : Cursor Correlation

If a vertical crosshair moves in window "a", the horizontal crosshair of
window "b" and the vertical crosshair of window "e" will move. If the
horizontal crosshair of window "a moves, the vertical crosshair of
window "d" and the horizontal crosshair of window "e" will move. The
crosshair in each window only tracks the motion of the moved crosshair
if the plot limits of the window overlap the position of the moved
crosshair. Crosshair tracking can be disabled in a window by changing
the window's axis label(s).

The mechanism by which cursors are correlated makes it important to use
a consistent scheme for labeling the various dimensions of experiments.
Also, multi-dimensional datasets should always have unique labels for
the different dimensions. A similar mechanism exists for displaying
peaks on spectra, so the need for consistent labeling of spectra, and
unique labeling within a dataset, is also necessary for the proper
rendering of peak displays. The best way to have cursors correlate and
peak markers display in an appropriate manner is to develop a consistent
labeling scheme, and stick with it.

And remember, there are two types of labels, one set with "label" and
one set with "dlabel". The former is used for things like crosshair
correlation as described here, and the later for the value that is
actually displayed on the spectrum.

### Using the Selector Cursor

Selector mode can be used when the cursor is in the "selector" mode.
Click the arrow button near the lower left corner of the window.

**To expand the spectrum view**

Press and hold the left mouse button with the cursor at the position you
want to start the expansion at. Keep the button down as you drag the
crosshair to a new position. As you drag the cursor a
blue box will be displayed to indicate the new region.
When you release the mouse button the
window will expand to display the selected region.  Initially the
blue box is drawn with dashed lines, you need to drag the box at
least big enough so that the lines are solid when you release the
mouse.  This requirement for dragging out at least a minimum sized
region minimzes the risk of accidental expansions.  Also, if you
change your mind about expanding the region you can just drag the
mouse back towards the origin.  Once the box is displayed with
dashed lines you can release the mouse button and no resizing will
be done.

**To move the spectrum region**

Hold down the Shift and the Alt keys together, and then
click and drag with the left mouse button. The spectrum will pan
left and right along with the cursor. With 2D spectra you can also pan
the spectrum region vertically.

Alternatively, you can move the spectrum region by
dragging the mouse while the cursor is positioned
within the left, to drag the y-axis,  or bottom, to drag the x-axis,
axis regions.

**To add or adjust a spectrum region**

Spectrum regions, used for integration etc., can be added to 
1D spectra. 
Use the same protocol as above to expand the view, but press and hold
the Alt key on the keyboard while performing the actions.
If you do this
in an area that doesn't overlap any previously existing regions, a new
region will be added to the spectrum. If the area does overlap a region,
then that region will be adjusted so the limits correspond to the
selected area.

When the region is added you'll see an integral line drawn above the 
added region.

**To select peaks**

If peak boxes are displayed on the spectrum, you can select the peaks
with the cursor in Selector mode.  Click on an individual peak box
to select it.  If this is a 1D spectrum, then click on the 
peak label drawn below the spectrum to select it.
Once selected, you can move the peak box on the spectrum
by clicking and dragging it.  You can resize the peak box by pressing
the Alt-key down before you start dragging the mouse

You can select multiple peaks by clicking and
dragging a box, as done with expansions or regions described above,
but with the Shift-key held down..
When you release the mouse button, all the peaks in the selection
box (displayed in yellow), will be selected.  As in the above modes,
if you release the mouse while the box border is drawn with dashed 
lines no action will be taken.


## Key Bindings

You can quickly navigate around spectra and peak-lists using keys on 
the keyboard. To use this feature the active window must have the
"focus", that is, it must be the last window you clicked the mouse in.

### Multi-key bindings

***Add peak***
These key sequence are used to add a peak at the position of the mouse.

**aa**

: Search for the local maxima and add a peak box there.  For
2D (contour) displays The cursor
must be positioned over a peak (contours displayed), but doesn't 
have to be exactly at the position of maximum intensity.

**as**

: Add a peak at the exact position of the mouse cursor.  There
doesn't have to be a peak displayed (local intensity above the 
display contour) at that position.

***Change cursor mode***
The cursor can be displayed in two (at present) modes, Crosshair
and Selector. The actions taken when clicking and dragging the
mouse depend on the cursor mode and these can be changed
with the following key bindings.

**c1**

: Change to single button mouse mode (both cursors can
be moved by pressing and dragging with the left mouse button down.

**c3**

: Change to three button mouse mode.  The black crosshairs
are moved with the left mouse button down, and the red
crosshairs moved with the middle mouse button down.

**cc**

: Change to the Crosshair cursor (from Selector).  Does not
change 1-button/3-button mode.

**cs**

: Change to the Selector cursor (from Crosshair).  Does not
change 1-button/3-button mode.

***Peak slider***
The peak slider is a tool that can be displayed at the bottom of the spectrum window
and is used in one of NMRFx's peak assignment modes.


**df**

: Freeze the currently selected peak. Frozen peaks
can no longer be slide, and their chemical shifts will
be sued to update that of the atoms assigned to 
each of the peaks dimensions.

**dt**

: Thaw the currently selected peak.  After thawing,
a previously frozen peak will be moveable again.

**ds**

: Tweak a peak box by sliding it into the postion of nearest
overlapping peak position. It will also be frozen.

**da**

: Add (show) the peak slider at bottom of current window.

**da**

: Quit (hide) the peak slider tool.


***Jump To(x,y,z,a)***
These key sequences allow you to quickly jump the spectrum view to specified plot limits. The jump key sequences start with a **j** key 
followed by a letter specifying the axis (x, y, ...) they act on.  The behaviour of some of the key patterns differ between the visible
axes (x and y) and planes (z, a ...).  In the following descriptions, the **?** stands for the axis name.  

**j?VALUE**

:   For axes representing planes (like **z**), this will jump the view to the spcified plane. If the VALUE  has a decimal point (**jz117.3**), then
the value represents a position in ppm.  If there is no decimal point (**jz32**), the value represents a plane number.  For visible axes (x and y), 
the view will jump to be centered on the specified value.  Because the number of characters is dependent on the specified value, you
need to end the value by pressing the Enter key.


**j?b**

:    Jump to the bottom (first) plane.  Not allowed for visible axes (x and y).


**j?c**

:    Jump to the center plane.  Not allowed for visible axes (x and y).


**jzf**

:    Set the plot limits (or range of planes) for the specified axis to the full range. 


**jzm**

:    Jump to the plane that has the maximum intensity at the position of the intersecting black crosshairs.  Useful when showing a range of
planes to jump to the plane with a visible peak.


**jzt**

:    Jump to the top (last) plane.  Not allowed for visible axes (x and y).




***Jump To(x,y,z,a)***
These key sequences allow you to quickly jump the spectrum view to specified plot limits. The jump key sequences start with a **j** key 
followed by a letter specifying the axis (x, y, ...) they act on.  The behaviour of some of the key patterns differ between the visible
axes (x and y) and planes (z, a ...).  In the following descriptions, the **?** stands for the axis name.  

**j?VALUE**

:   For axes representing planes (like **z**), this will jump the view to the spcified plane. If the VALUE  has a decimal point (**jz117.3**), then
the value represents a position in ppm.  If there is no decimal point (**jz32**), the value represents a plane number.  For visible axes (x and y), 
the view will jump to be centered on the specified value.  Because the number of characters is dependent on the specified value, you
need to end the value by pressing the Enter key.


**j?b**

:    Jump to the bottom (first) plane.  Not allowed for visible axes (x and y).


**j?c**

:    Jump to the center plane.  Not allowed for visible axes (x and y).


**jzf**

:    Set the plot limits (or range of planes) for the specified axis to the full range. 


**jzm**

:    Jump to the plane that has the maximum intensity at the position of the intersecting black crosshairs.  Useful when showing a range of
planes to jump to the plane with a visible peak.


**jzt**

:    Jump to the top (last) plane.  Not allowed for visible axes (x and y).

***Undo commands***
Changes in view (display region or contour level) can be undone and redone.
A history of changes is maintained so multiple actions can be undone and redone.

**uu""

: Undo last change.

**ur""

: Redo last undone change.


***View***
The View commands allow quickly changing the spectrum display plot limits.

**vc**

:    Center the spectrum at the position of the crosshair.  This moves the spectrum view, but doesn't change the overall plot range.


**ve**

:     Expand the view to represent the area inside the currently displayed crosshair box.


**vf**

:     Change the view to represent the full range of the current dataset.


**vi**

:    Zoom the view in (so it shows a smaller region of the dataset, centered on current view center).


**vo**

:    Zoom the view out (so it shows a larger region of the dataset, centered on current view center).


**vr**

:   Read Limits: Stores into a buffer the current plot limits of the
    window including the dataset dimensions assigned to each axis, and
    the chemical shift range displayed on each axis. Does not store
    parameters such as the assigned dataset, peak lists, colors etc. Use
    Copy/Paste (see above) for those parameters.


**vw**

:   Write Limits: Sets the plot limit parameters of the window to those
    store to the limits buffer with the read limits command (see above).


###  Arrow Keys

Use the cursor keys to move up or down planes in 3D and 4D spectra,
increment or decrement rows and columns in 1D displays of 2D,3D or 4D
spectra, change contour levels, and rotate spectra.  These keys are active
in both the legacy key binding and new (Extra) key binding modes.

**Down Arrow**

:   1Dx: Move up a row. 3D,4D Spectrum: Move Down a plane.

**Up Arrow**

:   1Dx: Move down a row. 3D,4D Spectrum: Move Up a plane.

**Left Arrow**

:   1Dy: Move left a column. 4D Spectrum: Move Down a Z2 plane.

**Right Arrow**

:   1Dy: Move right a column. 4D Spectrum: Move Up a Z2 plane.

**Control-Up Arrow**

:   Increase contour level.

**Control-Down Arrow**

:   Decrease contour level.

**Shift-Right Arrow**

:   Rotates the view of the spectrum by incrementing the dimension
    displayed on the y axis. For example, for a three-dimensional
    dataset, if the dataset dimensions displayed on the x, y and z axis
    are 1, 2 and 3, after this key-action, the dataset dimensions will
    be 1,3 and 2. Clicking again will rotate the view again, back to
    dimensions 1,2 and 3. Rotation is around the center of the currently
    displayed view, so that the new chemical shift of the z axis, is the
    value that was at the center of the previous y axis.

**Shift-Left Arrow**

:   Same as Shift-Right Arrow, but instead the dataset dimension on the
    y axis is decremented. The direction of rotation only matters if the
    dataset has more than three dimensions.

**Shift-Up Arrow**

:   Rotates the view of the spectrum by incrementing the dimension
    displayed on the x axis. For example, for a three-dimensional
    dataset, if the dataset dimensions displayed on the x, y and z axis
    are 1, 2 and 3, after this key-action, the dataset dimensions will
    be 3,2 and 1. Clicking again will rotate the view again, back to
    dimensions 1,2 and 3. Rotation is around the center of the currently
    displayed view, so that the new chemical shift of the z axis, is the
    value that was at the center of the previous x axis.

**Shift-Down Arrow**

:   Same as Shift-Down Arrow, but instead the dataset dimension on the x
    axis is decremented. The direction of rotation only matters if the
    dataset has more than three dimensions.

### Trackpads and scroll mice

Use the trackpad and scroll mouse to change display level and pan
through the spectrum. Trackpad use has only been tested on a Mac, but
may work on other operating systems.

**ScrollMouse Wheel**

:   Pan display region of the spectrum up and down.

**Control-ScrollMouse Wheel**

:   Scroll the mouse wheel with control key down to increase or decrease
    the contour display level (2D) or vertical scaling (1D).

**TrackPad**

:   Two fingered-swipe on the trackpad will pan the spectrum left/right
    and up/down with the direction corresponding to the swipe direction.

**Control-TrackPad**

:   Two fingered-swipe on the trackpad in the "vertical" direction will
    increase or decrease (depending on swipe direction) the contour
    display level (2D) or vertical scaling (1D).
