---
layout: blank
title: Three-column layout
breadcrumbs:
  - name: section
    url: section.html
  - name: sub-section
    url: sub-section.html
tags:
  - name: tag1
  - name: tag2
  - name: tag3
---

<!-- This is for content in the main container, outside of the grid row. -->
# This is a three-column layout

{% include breadcrumbs.html %}

{% include tags.html tag-settings="bg-secondary" container-settings="margin-y-5" %}

<!-- Content for the grid row begins here. -->

<!-- This is the content for column 1. -->
{% capture col1 %}
This could be some navigation:
- Section 1
- Section 2
- Section 3
{% endcapture %}

<!-- This is the content for column 2. -->
{% capture col2 %}
Prior to serving as the Director for BOEM, Amanda Lefton most recently served as the First Assistant Secretary for Energy and Environment for the Governor of New York where she led the State’s climate and environmental initiatives and managed a portfolio of twelve agencies and authorities. In this role she championed and advanced implementation of landmark nation leading climate and renewable energy strategies. Previously, Amanda was the Deputy Policy Director for The Nature Conservancy in New York, worked in the labor movement for the Rochester Regional Joint Board of Workers United, and for the New York State Assembly. She also worked for the State Senate.

Originally from Queens, NY, Ms. Lefton grew up on Long Island, NY, and holds a Bachelor of Arts from the University at Albany.
{% endcapture %}

<!-- This is the content for column 3. -->
{% capture col3 %}
**Email:** <Amanda.Lefton@boem.gov>{: .usa-link}

**Phone:** 202-208-6474

**Office:**<br>
Office of Public Affairs<br>
1849 C Street, NW<br>
Washington, D.C. 20240
{% endcapture %}

<!-- Convert the Markdown content for each column to HTML. -->
{% assign col1-formatted = col1 | markdownify %}
{% assign col2-formatted = col2 | markdownify %}
{% assign col3-formatted = col3 | markdownify %}

<!-- Put the HTML content into grid columns and add optional settings. -->
{% capture row %}
{% include column.html content=col1-formatted column-settings="grid-col-3" %}
{% include column.html content=col2-formatted column-settings="grid-col-6" %}
{% include column.html content=col3-formatted column-settings="grid-col-3" %}
{% endcapture %}

<!-- Put the grid columns into a grid row and add optional settings. -->
{% include row.html content=row row-settings="grid-gap" %}