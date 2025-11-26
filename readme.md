# Window Dimensions Tool
A simple tool that displays the current viewport dimensions with a resizable pixel grid and pointer position crosshairs. Meant to help web devs & designers get a visual for the scale of pixel dimensions on their screens.

***

## version 1.0 | Updated November 23, 2025
A simple tool that simply displays the current viewport dimensions with a resizable pixel grid and pointer position crosshairs. Meant to help web devs & designers get a visual for the scale of pixel dimensions on their screens.

> **Note:** Mobile/touch devices not yet supported.

**User Guide**
- Resize the window and view the current viewport dimensions in the "Window" property in the display box.
    > *Issue: On widow resize, new gridlines start at the last rendered viewport "x" dimension instead of at the correct grid spacing. Please refresh the page or modify the grid spacing to re-render properly.*
- Move the mouse around the viewport to see the mouse's current cartesian corrdinates in the display box.
- Click the mouse to toggle crosshairs.
- Use the checkmark to toggle the grid on/off.
- Enter a number from 10–8000 px in the "Grid Spacing" input. Optionally, use the incrementors to adjust.
    > *Issue: The suggestions dropdown acts as a search-suggestions instead of static selectable presets.*
    > *Issue: The dropdown & incrementor are invisible (dark-mode, not yet tested for light-mode)*
    > *Issue: The viewport doesn't account for the browser tab-bar, causing input to register at an 95px Y-offset when the page is scrolled to where the top of the document is at the top of the tab-bar (instead of the bottom, as would be desired) and the page to include 95px of scrollable area. (This tool was used to determine theese exact dimensions.)*
        > Note: *Tested in Chrome on android. Not yet tested in other browsers, or on iOS.*
        > Note: *This is a common issue for many pages on the web. Thus, this tool is accurate to common practice. I'm currently looking for ways to circumnavigate this quirk, and will add a toggle to fix this once I do.*

---

## version 1.1 | Updated November 24, 2025
**New Features**
- Mobile device viewport offset correction
- Touch input support
- Crosshair modes:
    - Follow mode: Original. Click to toggle on/off; crosshairs follow mouse.
    - Keep mode:
        - Touch/click & drag to move crosshairs around
        - Release to either keep or remove crosshairs (depending on mode)
        - Tap/click at cross to select crosshairs for delete/reposition