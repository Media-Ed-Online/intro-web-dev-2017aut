---
title: Viewport Units
module: 11
---

# Viewport Units

Another relative size unit, not yet discussed is viewport units. A viewport unit is either defined as `vh`, for height ratios, or `vw` for width ratios.

`1vh` is defined as 1/100th of the height of the viewport or browser. This means that `100vh` is the full height of the viewport window.

This can be particularly useful when working boxes that you want to be or maintain a height that is in relation to the height of your browser.

Likewise, `1vw` is 1/100th of the viewports width. However, you must be careful when working with `vw` units, as they are based on the width excluding scroll bars. On macOS this is not a problem, but on Windows, `100vw` will not fit in a browser, as the scroll bars will cause it to need to reflow. Therefore, you may be bast served to use percentages when setting width.

For more on this problem read; ["Viewport units: vw, vh, vmin, vmax" by Tim Severien](https://web-design-weekly.com/2014/11/18/viewport-units-vw-vh-vmin-vmax/)
