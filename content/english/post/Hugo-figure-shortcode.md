---
title: 'Hugo Figure Shortcode'
date: 2021-03-13T21:47:41+00:00
tags: 
- hugo
- shortcode
thumbnail: https://webse.nl/wp-content/uploads/2017/11/shortcode.jpg
---

Hugo has `figure` shortcode built-in, so you can easily add figure captions or hyperlink rel attributes to images. Documentations can be found here:

https://gohugo.io/content-management/shortcodes/#figure

This theme has **3 CSS classes** made for figure elements:

* `big`: images will break the width limit of main content area.
* `left`: images will float to the left.
* `right`: images will float to the right.

If a figure has no class set, the image will behave just like a normal markdown image: `![]()`.

Here are some examples; please be aware that these styles only take effect when the page width is over 1300px.

Input:
```md
{{</* figure src="https://images.unsplash.com/photo-1543169964-aee4453d2140?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" width="800" height="500" caption="Leiden bike (800×500，without any classes)" */>}}
```
Output:
{{< figure src="https://images.unsplash.com/photo-1543169964-aee4453d2140?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" width="800" height="500" caption="Leiden bike (800×500，without any classes)" >}}


{{< figure src="https://images.unsplash.com/photo-1543169964-aee4453d2140?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" width="800" height="500" class= "left" caption="Leiden bike (800×500，class is left)" >}}

Pellentesque posuere sem nec nunc varius, id hendrerit arcu consequat. Maecenas commodo, sapien ut gravida porttitor, dolor risus facilisis enim, eget pharetra nibh nisl porttitor sapien. Proin finibus elementum ligula sit amet hendrerit. Praesent et erat sodales ante accumsan pharetra non eu nulla. Sed vehicula consequat lorem, a fermentum ante faucibus quis. Aliquam erat volutpat. In vitae tincidunt dui. Proin sit amet ligula sodales, elementum tortor et, venenatis sem. Maecenas non nisl erat. Curabitur nec velit eros. Ut cursus lacus nisi, non pretium libero euismod et. Fusce luctus in nisi quis sollicitudin. Aenean nec blandit ligula. Duis ac felis lorem. Proin tellus tellus, dictum nec tempus sit amet, venenatis ac felis. Sed in pharetra nulla, non mollis sem.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-big" class="big" >}}


