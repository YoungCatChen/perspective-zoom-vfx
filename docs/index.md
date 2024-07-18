# PerspectiveZoom VFX

This is a visual effect plugin for DaVinci Resolve. It zooms your video natually
while keeping correct perspective.

(video with effect panel: mouse dragging zoom in, moves center to left, zoom
out, moves back to center)

## Installation

- Click on the latest release on the right-hand side column, then download the
  `PerspectiveZoom.drfx` file.
- Double click the downloaded file, wait while DaVinci Resolve is starting up,
  then it will ask you if you want to install this plugin in a popup window.
- Click “Install” and open any project, then you will find it in the Effects
  Library. Enjoy!

## Features

### Keep correct perspective

▼ Built-in transform: keeps wide-angle lens distortion

(video with effect panel: mouse moves pivot, zoom in, showing distorted image)

▼ This plugin: removes distortion

(video with effect panel: mouse moves center, zoom in, showing correct image)

### Zoom in natually at a smooth speed

▼ Built-in transform: zooms in quickly at first and slowly at last

(video: 0-1s: steady; frames with 200%, 400%, 800%, 1600%.
1-6s: 100% - 1600%, with text showing "zoom: x00%".
6-7s: steady)

▼ This plugin: zooms in at a constant speed

(video: 0-1s: steady; same frames.
1-6s: 100% - 1600%, with text showing "zoom: 2^x = y00%".
6-7s: steady)

▼ This plugin: ease-in / ease-out for zoom speed

(video like above. 1-6s: with ease in and out)

### Control zoom and pan natually

▼ Built-in transform: video sometimes moves out from frame

(video: 0-1s: steady.
1-4s: left to mid-left; highly zoom to mid zoom.
4-5s: steady)

▼ This plugin: just works as you would expect

(same video move)

### Transition without keyframes

The built-in transform effect requires to add keyframes to perform a complicated
transition. This plugin can work with _Adjustment Clips_ and make transition
much easier.

(video with timeline and effect panel.
zoom in left; move to right; zoom out.
add some blur.)
