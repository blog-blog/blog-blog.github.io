---
layout: post
title: "On Creating a Blog"
date: 2024-10-13 0:0:0
categories: digital-literacy-narrative
permalink: /projects/dln-4
---

This final part of my [Digital Literacy Narrative](../projects/dln) will be much less polished (if we can even call the previous 3 polished…)

I've used What You See Is What You Get (WYSIWYG) document processors for so long that creating this blog has been a major obstacle! I know markdown and HTML and CSS to a degree, but I had to figure out the basics of Jekyll. Thankfully, it's much easier to make a Jekyll site on Github than it is on Gitlab (which I tried using, at first).

One of the major obstavles was image placement. At first, I was using a weird double-column system using CSS grid attributes. At its worst, it looked a little something like this:

```html
<div style="display:grid;grid-template-columns:1fr 1fr">
<div>
<p>
Imagine a cold, wet, gloomy …
</p>
<p>
Also think of a warm home, …
</p>
<p>
Representing a break from school, time with family, and the winter-Christmas aesthetic, these times in my childhood were always important.
</p>
</div>
<div style="padding:0 0 0 2rem">
<figure>
<img src="/assets/media/winter_illinois.jpg" alt="my alt text"/>
<figcaption>
Taken one winter in Illinois, overlooking the [Mazon Creek](https://en.wikipedia.org/wiki/Mazon_River).
</figcaption>
</figure>
<figure>
<img  src="/assets/media/christmas_cookies.jpg" alt="my alt text"/>
<figcaption>
Christmas sugar cookies, the cookies made by me and decorations done together.
</figcaption>
</figure>
</div>
</div>
```

This same section now looks like this:

```markdown
<div>
<figure>
![Picture from a bridge overlooking an icy creek and snowy trees](/assets/media/008.jpg)
<figcaption>
Taken one winter in Illinois, overlooking the [Mazon Creek](https://en.wikipedia.org/wiki/Mazon_River).
</figcaption>
</figure>
<figure>
![A spread of sugar cookies decorated in red, green, and white royal icing](/assets/media/003.jpg)
<figcaption>
Christmas sugar cookies, the cookies made by me and decorations done together.
</figcaption>
</figure>
</div>
{: .image-right}
```

At minimum, a right-aligned image looks like this:

```
![](image-location)
{: .image-right}
```

All thanks to helpful Kramdown features, Jekyll's flavor of markdown!

I also had to figure out how Jekyll's styling works as I wanted to change the default look quite a bit. I began this project with Hugo, but I couldn't figure out how to customize it. I changed the backgrounds and most notably the font to [Inter](https://rsms.me/inter/).
