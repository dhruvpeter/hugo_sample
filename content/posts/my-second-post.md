---
title: "My Second Post"
date: 2021-06-22T15:46:16+05:30
draft: false
tags: ["yolo"]
---
Second page

<h5>html codes in md files are working</h5>

### Given below are some examples using shortcodes

<!--
Sample button
!-->
{{< button "Go to first post" "/posts/my-first-post/">}}

{{< button "Click here to know more about shortcodes" "https://gohugo.io/content-management/shortcodes/">}}
<!--
Sample shortcode where color is passed as parameter.
The text dispayed is given in the shortcode template
!-->
{{< sampleshortcode color="blue">}}

<!--
Here text is passed, the highlighting is done using shortcode
!-->
{{< custom_highlight >}}
 This is highlighted using shortcode
{{< /custom_highlight >}}


<!--
This is a default shortcode available with hugo
!-->
{{< highlight go >}} Highlight using default shortcode {{< /highlight >}}

<!--
This can be used to render markdown text
!-->
{{% mdshortcode %}}
This is markdown text using **shortcodes**
{{% /mdshortcode %}}
<!--
This is also a default shortcode available with hugo
!-->
**Youtube video below is embedded using shortcode**
{{< youtube BvdlZsK5ZWY>}}
