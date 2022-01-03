---
layout: default
title: Home
---
# {{ site.title }}

{{ site.description }}
{: .usa-intro}

{% include text-input.html label="First name" id="first-name" input-tokens="bg-light border-accent-cool border-05" label-tokens="text-bold" %}

## Choose dates

{% include date-picker.html label="Start date" id="start-date" hint="mm/dd/yyyy for when it starts" %}

{% include date-picker.html label="End date" id="end-date" hint="mm/dd/yyyy for when it ends" %}


<!-- Create alert content as Markdown between these capture tags. -->
{% capture alert-text-markdown %}
Lorem ipsum dolor sit amet, [consectetur adipiscing elit](#), sed do eiusmod.
{: .margin-y-0}
<!-- Optional utility token to remove top and and bottom margin from body paragraph. -->
{% endcapture %}

<!-- This converts the Markdown content above into HTML for transferring to the component include below. -->
{% assign alert-text-html = alert-text-markdown | markdownify %}

<!-- The alert include using the converted HTML content. -->
{% include alert.html heading="Houston, we have a problem" variant="warning" content=alert-text-html %}

<!-- This is a simple alert that only allows plain-text for the body paragraph -->
{% include alert-simple.html heading="Houston, we have a problem" variant="info" content="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod." %}