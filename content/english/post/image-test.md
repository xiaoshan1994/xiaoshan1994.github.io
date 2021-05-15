+++
author = "Hugo Authors"
title = "Guide to Thumbnails in Hugo"
date = "2019-03-04"
description = "Guide to Thumbnails in Hugo"
tags = [
    "thumbnail",
]
thumbnail= "{{< figure src=
"https://chi01pap002files.storage.live.com/y4mEneJaDZPSUbm01spsuyu0kwDU8_12umJQKJBZMPwzbNMCJ28Jon0zI6hWM2rJW5IqRqFPyTIO_hWHVwvEscbmcd9tvhM9jW1vm0vp79I3HDm2d6QiWeXauiP8Q9aKXxdUPvCh66GbCOWdKNVgYcyFRvEZyweWHM7c4xLYmX_2eKUd7BT3nHMgPwqXmtMaGu?width=1001&height=624&cropmode=none" >}}"
+++
Thumbnails can be enabled easily by setting the `thumbnail` parameter in the frontmatter to an image such as `"images/landscape.jpg"`. 

Make sure to copy the image the `static/images/` directory.

If put together, it will look like this (that's in fact this post's frontmatter):

```md
+++
author = "Hugo Authors"
title = "Guide to Thumbnails in Hugo"
date = "2019-03-04"
description = "Guide to Thumbnails in Hugo"
tags = [
    "thumbnail",
]
thumbnail= "images/landscape.jpg"
+++
```


