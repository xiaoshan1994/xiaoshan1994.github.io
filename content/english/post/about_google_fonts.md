---
date: 2021-05-17
title: Changing Fonts in hugo website
description: Thanks to Damien. I got new hugo shortcodes for the fonts update in this website.
tags:
- hugo shortcodes
- fonts
Categories:
- Website
thumbnail: https://www.lifewire.com/thmb/PBDyu2zoMIy3mya-QIgbxF587xs=/2201x1362/filters:no_upscale():max_bytes(150000):strip_icc()/GettyImages-157679986-5b2ed453a474be0036cf7d58.jpg
images: https://www.lifewire.com/thmb/PBDyu2zoMIy3mya-QIgbxF587xs=/2201x1362/filters:no_upscale():max_bytes(150000):strip_icc()/GettyImages-157679986-5b2ed453a474be0036cf7d58.jpg
---
Thanks to Damien. I got new hugo shortcodes for the fonts update in this website.
<!--more-->
Google Fonts is a great library of free fonts that you can use
on your sites.

Normally, you have to edit a bunch of
html files with repeated codes - but now
you only need to make a hugo shortcode
and save it in your `layouts/shortcodes` file.

 The code script for my site:

 ```md
{{ $font := .Get "font" }}
{{ $size := .Get "size" }}
{{ $style := .Get "style" | default "normal" }}
{{ $weight := .Get "weight" | default "normal" }}
<link href="https://fonts.googleapis.com/css?family={{$font }}" rel="stylesheet" type="text/css">
<div style="font-family:'{{ $font }}'; font-size:{{ $size }}; font-style:{{ $style}}; font-weight:{{ $weight }}">
    {{- .Inner -}}
</div>
```
How to use it
```md
{{</* gfont font="font-family" size="36px" weight="bold" */>}}
You are awesome. You're even better!
{{</* /gfont */>}}
```
You can customize the shortcode name which should be the same with the file name (without extension). Pay attention to the the closing part `{{/* gfont */}}`.

Here are some examples I hope to deploy in this blog site:

For posts of **daily life** (`Pattaya`and `Courgette`):

```md
{{</* gfont font="Pattaya" size="30px" */>}}
Pattaya is a city in Thailand.<br>A beach resort popular with tourists.
{{</* /gfont */>}}
{{</* gfont font="Courgette" size="15px" */>}}
Courgette works well in smaller sizes and even in text.
{{</* /Courgette */>}}
```
{{< gfont font="Pattaya" size="30px" >}}
Pattaya is a city in Thailand
{{< /gfont >}}

{{< gfont font="Courgette" size="15px" >}}
Courgette is a medium-contrast, brushy, italic-script typeface. The genre is traditionally used at large sizes but Courgette was carefully made for the web, with low stroke contrast that works well in smaller sizes and even in text.
{{< /gfont >}}

For **English learning posts** (`Bangers` and `Kalam`):
 ```md
 {{</* gfont font="Bangers" size="30px" */>}}
 Bangers is a comicbook style
 {{</* /gfont */>}}

 {{</* gfont font="Kalam" size="15px" */>}}
 Kalam is a handwriting font family that supports the Devanagari and Latin writing systems. Even though Kalam's letterforms derive from handwriting, the fonts have each been optimized for text usage on screen. All in all, the typeface is a design that feels very personal. Like many informal handwriting-style fonts, it appears rather fresh and new when seen on screen or printed on the page.
 {{</* /gfont */>}}
 ```

{{< gfont font="Bangers" size="30px" >}}
Bangers is a comicbook style
{{< /gfont >}}

{{< gfont font="Kalam" size="15px" >}}
Kalam is a handwriting font family that supports the Devanagari and Latin writing systems. Even though Kalam's letterforms derive from handwriting, the fonts have each been optimized for text usage on screen. All in all, the typeface is a design that feels very personal. Like many informal handwriting-style fonts, it appears rather fresh and new when seen on screen or printed on the page.
{{< /gfont >}}

For types of **literature or technology**(`Oswald`and `Roboto`)

 ```md
{{</* gfont font="Oswald" size="30px" */>}}
Oswald is one of the new comers to this long tradition.
{{</* /gfont */>}}

{{</* gfont font="Roboto" size="15px" */>}}
Roboto has a dual nature. It has a mechanical skeleton and the forms are largely geometric. At the same time, the font features friendly and open curves.
{{</* /gfont */>}}
```

{{< gfont font="Oswald" size="30px" >}}
Oswald is one of the new comers to this long tradition.
{{< /gfont >}}

{{< gfont font="Roboto" size="15px" >}}
Roboto has a dual nature. It has a mechanical skeleton and the forms are largely geometric. At the same time, the font features friendly and open curves.
{{< /gfont >}}
