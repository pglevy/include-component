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