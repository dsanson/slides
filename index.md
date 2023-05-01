---
title: Example Slideshow
author: David Sanson
institute: Illinois State University
---

# Screencast Slideshows

A setup for recording screencast slideshows with video, using reveal.js. Trying to mimic some of the simple effects (overlays, transitions) of OBS without the overhead.

# Basic Ideas

-   use built-in screencast recording to record browser window with webcam displayed.
-   use custom slide layouts to integrate webcam into slide content in different ways.
-   use reveal.js animations for simple "overlay" effects.

# reveal-embed-video.js

-   using <https://github.com/ThomasWeinert/reveal-embed-video>
-   .js updated to register properly as a plugin for Revealjs 4.0
-   .css modified to add additional video placement (move to overlay.scss?)

# screencast.scss

-   layouts designed to be used with webcam video
    -   overlay layouts: for displaying *over* webcam video
    -   TODO: grid/flex layouts that integrate webcam into slide layout 
-   TODO: include carnap exercises in slides
-   TODO: styles/animations that mimic OBS overlays

# Demo {video="full"}

-   Press 'S' to view speaker notes, which include explanations.
-   Press 'C' to enable the camera.

# Fullscreen camera {video="full"}

Camera displays under content.

:::notes
Fullscreen webcam under slide layout. Meant for use either with empty slides, or with overlay layouts.
:::


# Lefthalf camera {video="left"}

Camera displays under content.

:::notes
For use with an overlay layout with a solid background on the right for focused content.
:::

# Overlay style {.overlay video="full"}

-   title bottom left
-   content top right

:::notes
The simple 'overlay' slide layout is meant to work well when drawn over the top of background video. The header is shifted to bottom left, and the content to the top right. Works best if speaker is positioned in left-hand side of video frame.
:::

# "Key Ideas" {.overlay .keys video="full"}

> -   layouts
> -   css
> -   reveal.js

:::notes
WIP. The idea is to present ul's as incrementally revealed "key ideas" while talking. Useful for introducing new ideas for the first time. Idea is to add more animation to make each keyword pop out as revealed.
:::

# No Video {video="false"}

Set the `video` attribute to false in order to disable video on a given slide.

# Other ideas {video="false"}

-   animate/emphasize defined terms: maybe enlarge and wobble?
-   add a chalkboard plugin to draw on slides

# That's all for now

BYE!

