---
layout: default
title: Director of BOEM Amanda Lefton
---

# {{ page.title }}

<!-- Create column content -->

{% capture column-1 %}
![Headshot photo of Amanda Lefton with the American flag in the background](https://raw.githubusercontent.com/Bixal/rrt-content/main/assets/img/Bio-LeftonAmanda.jpg)
{% endcapture %}

{% capture column-2 %}
Prior to serving as the Director for BOEM, Amanda Lefton most recently served as the First Assistant Secretary for Energy and Environment for the Governor of New York where she led the State’s climate and environmental initiatives and managed a portfolio of twelve agencies and authorities. In this role she championed and advanced implementation of landmark nation leading climate and renewable energy strategies. Previously, Amanda was the Deputy Policy Director for The Nature Conservancy in New York, worked in the labor movement for the Rochester Regional Joint Board of Workers United, and for the New York State Assembly. She also worked for the State Senate.
{: .margin-top-0}

Originally from Queens, NY, Ms. Lefton grew up on Long Island, NY, and holds a Bachelor of Arts from the University at Albany.

**Email:** <Amanda.Lefton@boem.gov>{: .usa-link}

**Phone:** 202-208-6474

**Office:**<br>
Office of Public Affairs<br>
1849 C Street, NW<br>
Washington, D.C. 20240
{% endcapture %}

<!-- Format the content for includes -->

{% assign column-1-formatted = column-1 | markdownify %}

{% assign column-2-formatted = column-2 | markdownify %}

<!-- Capture the columns for the row include -->

{% capture row %}

{% include column.html content=column-1-formatted column-style="grid-col" %}

{% include column.html content=column-2-formatted column-style="grid-col" %}

{% endcapture %}

<!-- Include the row with the formatted column content -->

{% include row.html content=row %}