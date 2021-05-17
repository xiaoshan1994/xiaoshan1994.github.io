---
date: 2021-05-17
title: 'changing Fonts in hugo website'
tags:
- hugo shortcodes
- fonts
Categories:
- Website
---

Thanks to [Damien](https://damien.co/blog/2020-06-20-use-custom-fonts-typography-hugo-shortcode/).
I got new hugo shortcodes for the
fonts update in this website.

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
{{< gfont font="font-family" size="36px" weight="bold" >}}
You are awesome. You're even better!
{{< /gfont >%}}
```
You can customize the shortcode name which should be the same with the file name (without extension). Pay attention to the the closing part `{{< /gfont >%}}`.

Here are some examples I hope to deploy in this blog site:

For quotations or references:
```md
> {{< typography font="monoton" size="10px" weight="bold",style="italic" >}}
You are awesome.
You're even better!
{{< /typography >%}}
```
> {{< typography font="monoton" size="10px" weight="bold",style="italic" >}}
> You're even better!
> {{< /typography >%}}

 Text for catching people's eyes:
