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
I am a masters student at York University studying Computer Science and supervised by Enamul Hoque Prince. Prior to this I completed my Bachelor's of Science in Computer Science at Toronto Metropolitan University (formerly Ryerson) and minored in Mathematics. My research is interdisciplinary and looks at the areas of **Human Computer Interaction**, **Natural Language Processing**, and **Data Analytics and Visualization**. Specifically, I am focused on building multi-agentic frameworks, creating related benchmarks, and creating empirical foundations for Vision Language Model based agents in their abilities to reason and traverse through interactive visualizations such as dashboards.  

 
Publications
======
1. DashboardQA: Benchmarking Multimodal Agents for Question Answering on Interactive Dashboards
2. Chartqapro: A more diverse andchallenging benchmark for chart question answering.
3. Chartgemma: Visual instructiontuning for chart reasoning in the wild.

 
## Recent Papers

{% assign pubs = site.publications | sort: "date" | reverse %}

{% for pub in pubs %}
<div style="display:flex; align-items:flex-start; margin-bottom:1.5rem;">

  {% if pub.image %}
  <div style="margin-right:1rem;">
    <img src="{{ pub.image | relative_url }}"
         alt="{{ pub.title }}"
         style="width:120px; max-width:120px; border-radius:4px;">
  </div>
  {% endif %}

  <div>
    <p style="margin:0;">
      <strong>{{ pub.title }}</strong><br>
      {{ pub.authors }}<br>
      <em>{{ pub.venue }}</em>, {{ pub.date | date: "%Y" }}
    </p>

    {% if pub.paperurl %}
    <p style="margin-top:0.5rem;">
      <a href="{{ pub.paperurl }}"
         style="border:1px solid #000; padding:3px 8px; text-decoration:none; font-size:0.85rem;">
        PDF
      </a>
    </p>
    {% endif %}
  </div>

</div>
{% endfor %}
