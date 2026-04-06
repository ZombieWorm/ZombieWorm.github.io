---
layout: page
title: Performance Benchmarks
permalink: /benchmarks.html
---

<h2 class="section-title">Quantised Models using an RTX 5080</h2>

<p>
  <strong style="color: var(--text)">Metrics</strong>: tokens/sec, VRAM usage, quality degradation<br> 
  <strong style="color: var(--text)">Setup</strong>: Llama.cpp | Various models tested
</p>
  
<div class="model-comparison">
  <!-- This wrapper allows the table to swipe left/right on mobile -->
  <div class="table-wrapper">
    <table aria-describedby="statusTableCaption">
      <caption id="statusTableCaption" style="color: var(--text-dim); font-size: 0.8rem; margin-bottom: 1rem;">
        Model Performance and Status Tracking
      </caption>
      <thead scope="colgroup">
        <tr role="row">
          <th scope="col">Model</th>
          <th scope="col">Summary</th>
          <th scope="col">Tool</th>
          <th scope="col">Prompt speed</th>
          <th scope="col">t/s</th>
          <th scope="col">VRAM usage</th>
          <th scope="col">Source</th>
          <th scope="col">Type</th>
        </tr>
      </thead>
      <tbody role="rowgroup">
        {% for item in site.data.model_statuses.models %}
        <tr role="row">
          <td role="cell">{{ item.model }}</td>
          <td role="cell">{{ item.summary }}</td>
          <td role="cell">{{ item.tool }}</td>
          <td role="cell">{{ item.prompt_speed }}</td>
          <td role="cell">{{ item.tokens_per_second }}</td>
          <td role="cell">{{ item.vram_usage }}</td>
          <td role="cell">{{ item.source }}</td>
          <td role="cell">{{ item.type }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
</div>
