---
layout: project.pug
title: Wahila Creative Accessibility Checker
preview: "At Wahila Creative we're committed to continually improving the accessibility of our websites. We built this internal tool to expedite automated testing, as we use four unique APIs to test WCAG2 compliance."
preview2: "We use this tool (in addition to human testing) both during the development process and in regular intervals post-launch to ensure the best experience for all users."
---

Early on, we realized that running four accessibility APIs against every page in a site would not only be tedious, but it would produce overlapping results for errors in common site elements such as navigation blocks. To solve this, [Wahila Creative](http://www.wahilacreative.com) decided to build a tool to aggregate the results of each API across multiple pages. The checker can be run against a single page or a list of pages; we leave site spidering to the APIs themselves when we need a full site analysis. APIs can also be turned on and off as a cost-saving measure for those which are paid services.

![alt text][search]

We produce an executive summary of the API information displaying the number of pages analyzed, number of total errors, and number of total warnings. These numbers are then broken down by WCAG checkpoint number and displayed in a table to visualize problem areas and differences between APIs. We also compile the most frequently failed checkpoints into a list, giving developers an easy place to start tackling accessibility problems.

![alt text][analysis]

Finally, the entire list of warnings and errors is displayed by page. Each item contains the checkpoint(s) failed, the inaccessible code in question, and information about the problem.

![alt text][error]

This project is powered by a MEAN stack sitting on a Digital Ocean droplet. We use the Tenon, aXe, pa11y, and AChecker APIs to run our automated tests.

[search]: /img/accessibility-home.png "An example of the Wahila creative accessibilty checker tool. The page displays a site search bar and options to select which APIs are used to test the accessibility of that site."
[analysis]: /img/accessibility.png "The results of testing a single page with the Wahila Creative accessibility checker tool. The page displays the number of warnings, errors, pages tested, and APIs used in the test."
[error]: /img/single-error.png "An example of a single accessibiity error within the Wahila Creative accessibility checker tool. This error states that an item on the page is too small to be reliably touched on mobile devices."
