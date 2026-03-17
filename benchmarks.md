---
layout: default
title: Benchmarks
permalink: /benchmarks/
---

# Benchmarks & Experiments

Real-world measurements from my local LLM & GPU setups.

<h1>Benchmarks</h1>

<ul>
  {% for item in site.benchmarks %}
    <li>
      <strong>{{ item.title }}</strong><br>
      <a class="btn" href="{{ item.url }}">View</a>
    </li>
  {% endfor %}
</ul>

<div class="grid">
  {% for item in site.benchmarks reversed %}
    {% include project-card.html project=item %}   <!-- reuse your existing card, or make benchmark-card.html -->
  {% endfor %}
</div>