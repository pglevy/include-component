---
layout: row
---

{% capture col1 %}
18F can help agencies with the process of developing an effective data strategy. Our principles of user-centered design, agile, and iterative delivery can increase your agencies’ chance for success in using data more effectively.
{: .usa-intro}

The Federal Government is one of the world’s biggest data producers. Finding, accessing, using, reusing, and protecting this data are challenges for which there have been several different initiatives during the past decade. The latest initiative is the [Federal Data Strategy](https://strategy.data.gov/){: .usa-link}, which provides a set of data principles and best practices in implementing data innovations that drive value for the public. This strategy includes an annual action plan for establishing processes, building capacity, and aligning existing efforts. Despite these guidelines and plans, it can be hard to know where to start when putting together a data strategy for your agency or organization.

18F can assist agencies interested in developing a data strategy. Making a plan to effectively use data is rarely straightforward, and involves technical skills, excellent communication, change management, and iterative development.
{% endcapture %}


{% capture col2 %}
The 18F team has experience in this area. We have:

- Assisted the Treasury Department [implement the DATA ACT](https://18f.gsa.gov/2016/06/14/prototype-early-prototype-often-lesson-from-the-data-act/){: .usa-link}
- Helped federal laboratories [organize and share their data more effectively](https://18f.gsa.gov/2017/10/05/18f-and-federal-laboratories-work-together-to-bring-better-data-to-businesses/){: .usa-link} with industry partners
- [Saved time and improved data quality](https://18f.gsa.gov/2020/04/23/saving-time-and-improving-data-quality-for-the-national-school-lunch-breakfast-program/){: .usa-link} for the National School Lunch & Breakfast Program.
- Worked with many other agencies to help create sustainable data practices. We discuss some highlights of these projects below.

We know from experience that each agency has diverse needs, resources, and maturity around data stewardship and related data skills.

We believe that [our principles and methods for working with agencies](https://18f.gsa.gov/partnership-principles/){: .usa-link} are ideal for assisting with the challenges of developing a forward-thinking data strategy.

Our approach to data projects is summed up in these principles:

1. Understand the problem
2. Let users be the guideposts
3. Work in an agile way
4. Leverage open resources
{% endcapture %}

<!-- Format the Markdown content above -->
{% assign col1-formatted = col1 | markdownify %}

{% assign col2-formatted = col2 | markdownify %}

<!-- Put the formatted content into separate columns in the grid. -->
{% include column.html content=col1-formatted %}

{% include column.html content=col2-formatted %}