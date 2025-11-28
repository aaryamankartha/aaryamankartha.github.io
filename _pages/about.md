---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

About me 
======
I am a masters student at York University studying Computer Science and supervised by Enamul Hoque Prince. Prior to this I completed my Bachelor's of Science in Computer Science at Toronto Metropolitan University (formerly Ryerson) and minored in Mathematics. My research is interdisciplinary and looks at the areas of Human Computer Interaction, Natural Language Processing, and Data Analytics and Visualization. Specifically, I am focused on building multi-agentic frameworks, creating related benchmarks, and creating empirical foundations for Vision Language Model based agents in their abilities to reason and traverse through interactive visualizations such as dashboards.  

 
Publications
======
1. DashboardQA: Benchmarking Multimodal Agents for Question Answering on Interactive Dashboards
2. Chartqapro: A more diverse andchallenging benchmark for chart question answering.
3. Chartgemma: Visual instructiontuning for chart reasoning in the wild.

 
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
