---
layout: blank
body-style: margin-top-5 bg-base-lighter
---

<!-- Capture Markdown content for use with `grid` component. -->
{% capture column %}
# Sign in to your account
{: .margin-top-0 .line-height-heading-2}

<!-- Use a `text input` component for username. -->
{% include text-input.html label="Username" id="username" type="text" %}

<!-- Use a `text input` component for password. -->
{% include text-input.html label="Password" id="password" type="password" %}

[Send me a link instead](#){: .usa-link}

[Sign in](home.md){: .usa-button .usa-button--accent-cool .width-full}

Don't have an account? [Create one](#)
{% endcapture %}

<!-- Convert the Markdown content to HTML. -->
{% assign column-html = column | markdownify %}

<!-- Put the HTML content into a grid column and add optional settings. -->
{% capture row %}
{% include column.html content=column-html column-style="tablet:grid-col-6 tablet:grid-offset-3 bg-white radius-lg padding-5 shadow-2" %}
{% endcapture %}

<!-- Put the grid column into a grid row and add optional settings. -->
{% include row.html content=row %}