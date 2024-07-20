# PerspectiveZoom VFX

This is a visual effect plugin for DaVinci Resolve. It zooms your video natually
while keeping correct perspective.

(video with effect panel: mouse dragging zoom in, moves center to left, zoom
out, moves back to center)

<style>
  video {
    margin-bottom: 1.5em;
  }
</style>

## Installation

1. Click on the latest release on the right-hand side column, then download the
   `PerspectiveZoom.drfx` file.
2. Double click the downloaded file, wait while DaVinci Resolve is starting up,
   then it will ask you if you want to install this plugin in a popup window.
3. Click “Install” and open any project, then you will find it in the Effects
   Library. Enjoy!

## Features

### Keep correct perspective

▼ Built-in transform: keeps wide-angle lens distortion [^persp]

<video controls muted width="720">
  <source src="perspective1.mp4" type="video/mp4" />
</video>

▼ This plugin: removes distortion [^persp]

<video controls muted width="720">
  <source src="perspective2.mp4" type="video/mp4" />
</video>

### Zoom in natually at a smooth speed

▼ Built-in transform: zooms in quickly at first and slowly at last [^zoom]

<video loop controls muted width="540">
  <source src="zoom1.mp4" type="video/mp4" />
</video>

▼ This plugin: zooms in at a constant speed [^zoom]

<video loop controls muted width="540">
  <source src="zoom2.mp4" type="video/mp4" />
</video>

▼ This plugin: ease-in / ease-out for zoom speed [^zoom]

<video loop controls muted width="540">
  <source src="zoom3.mp4" type="video/mp4" />
</video>

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


[^persp]: Image source: https://people.csail.mit.edu/yichangshih/wide_angle_portrait/webpage/additional-results/

[^zoom]: Image source: https://www.photos-public-domain.com/2012/03/25/pair-of-geese-on-the-water/
