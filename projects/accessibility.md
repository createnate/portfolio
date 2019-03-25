---
layout: project.pug
title: Wahila Creative Accessibility Checker
preview: "At Wahila Creative we're committed to continually improving the availability and accessibility of our websites to all users. We built this internal tool to expedite automated testing, as we use four unique APIs to test WCAG2 compliance."
---

Early on, we realized that running four accessibility APIs against every page in a site would not only be tedious, but it would produce overlapping results for errors in common site elements such as navigation blocks. To solve this, [Wahila Creative](http://www.wahilacreative.com) decided to build a tool to aggregate the results of each API across multiple pages. The checker can be run against a single page or a list of pages; we leave site spidering to the APIs themselves when we need a full site analysis. APIs can also be turned on and off as a cost-saving measure for those which are paid services.

![alt text][search]

We produce an executive summary of the API information in a 

![alt text][analysis]

Powering this project is a MEAN stack sitting on a Digital Ocean droplet. 

[search]: /img/accessibility-home.png "Search"
[analysis]: /img/accessibility.png "Analysis"
