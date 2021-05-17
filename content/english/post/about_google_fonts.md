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
{{</* gfont font="font-family" size="36px" weight="bold" */>}}
You are awesome. You're even better!
{{</* /gfont */>}}
```
You can customize the shortcode name which should be the same with the file name (without extension). Pay attention to the the closing part `{{/* gfont */}}`.

Here are some examples I hope to deploy in this blog site:

For posts of the daily life (`Pattaya`):

```md
{{</* gfont font="Pattaya" size="30px" weight="bold" style="italic" */>}}
Pattaya is a city in Thailand.<br>A beach resort popular with tourists.
{{/* gfont */}}
```

{{< gfont font="Pattaya" size="30px" >}}
Pattaya is a city in Thailand.<br>A beach resort popular with tourists.
{{< /gfont >}}

For English learning posts (`Architects Daughter` and `Courgette`):
 ```md
 {{</* gfont font="Architects Daughter" size="30px" */>}}
 Inspired by the writing of the daughter of an architect.
 {{</* /gfont */>}}
 {{</* gfont font="Courgette" size="15px" */>}}
 Courgette works well in smaller sizes and even in text.
 {{</* /Courgette */>}}
 ```

{{< gfont font="Architects Daughter" size="30px" >}}
Inspired by the writing of the daughter of an architect.
{{< /gfont >}}
{{< gfont font="Courgette" size="15px" >}}
Courgette works well in smaller sizes and even in text.
{{< /Courgette >}}
 For tedious literature🙈()
