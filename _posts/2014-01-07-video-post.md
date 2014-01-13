---
layout: post
type:	video
title: "A Post with a Video"
category: videos
tags: [sample post, video]
image: 
  feature: picture-21.jpg
comments: true
share: true
---

<iframe width="940" height="529" src="//www.youtube.com/embed/CQJByFp7H38?theme=light&amp;color=white" frameborder="0" allowfullscreen></iframe>


Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).

Not sure if this only effects Kramdown or if it's an issue with Markdown in general. But adding YouTube video embeds causes errors when building your Jekyll site. To fix add a space between the `<iframe>` tags and remove `allowfullscreen`. Example below:

{% highlight html %}
<iframe width="940" height="529" src="//www.youtube.com/embed/CQJByFp7H38?theme=light&amp;color=white" frameborder="0" allowfullscreen> </iframe>
{% endhighlight %}