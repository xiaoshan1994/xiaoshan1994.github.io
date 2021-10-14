---
date: 2021-05-17
title: 'Make Your Website Social Media Card'
description: 'This blog is transported from Rana Emad on DEV about the social card making'
tags:
- Hugo
- coder
categories:
- skill
images:
- https://res.cloudinary.com/practicaldev/image/fetch/s--3yJkrb96--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/y44m89pi90bi8p6g50lc.png
thumbnailImage:  https://res.cloudinary.com/practicaldev/image/fetch/s--3yJkrb96--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/y44m89pi90bi8p6g50lc.png
---
## Make Your Website Social Media Card-able on Twitter, Facebook and More

[See the original link](https://dev.to/ranaemad/make-your-website-social-media-card-able-on-twitter-facebook-and-more-35la#card-image-best-practices)

We all want our websites to be shared on Twitter, Facebook and all the different channels of social media. Whether they are our own websites that have our blogs and profiles or websites we built for other people. We all value those valuable clicks, so as a means of seduction to make our links clickable, we need to make them look attractive and pretty.

Instead of just sharing a bare link that doesn't give us enough indication of what the page content is about, we can turn it into a beautiful card that represents the content on each page of our website.

## Open Graph

Years ago, Facebook granted us Open Graph to turn our links into lovely rich graph object that can be shared easily and beautifully. Open Graph uses meta tags to communicate with our website and grab the desired information we want displayed in our cards. You can know more about it on the Open Graph Protocol website.

They are also not only available for Facebook, they are widely used and are available for Twitter, LinkedIn, Pinterest and many more social media platforms.

## Meta Tags

In order to build our cards, we have to pass our desired data through meta tags. We have lots of meta tags and you can find them all [HERE](https://ogp.me/), but if we're going to talk about the basic meta tags that are capable of making our card look good, then we have to mention the following 4 required tags:
* `og:title`

  Your title of choice
* `og:type`

  Whether it is a website or a video or an audio, ...etc. See Hugo font matter configuration [HERE](https://gohugo.io/templates/internal/). They call it "internal templates".
* `og:image`

  The image you would like to display on your card and we're going to talk later about its [dimensions and best practices](https://dev.to/ranaemad/make-your-website-social-media-card-able-on-twitter-facebook-and-more-35la#card-image-best-practices) for different socail media.
* `og:url`

  The URL you want displayed in the card.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--Pix_2neS--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://cdn.hashnode.com/res/hashnode/image/upload/v1594392173761/CsZCJnrG0.png)

## Where?

Once we open our head tag in our HTML structure, we can include all the meta tags we want.

```md
<head>
    <meta property="og:title" content="I am a title" />
    <meta property="og:type" content="website" />
    <meta property="og:url" content="IamAUrl.yes" />
    <meta property="og:image" content="imageURL.cool" />
</head>
```
Since the meta tag in HTML is different bwtween twitter and other platforms, I inserted into two hugo internal temmplates. It looks like this:

```md
<!-- Twitter Cards -->
{{ template "_internal/twitter_cards.html" . }}

<!-- Open Graph -->
{{ template "_internal/opengraph.html" . }}
```
