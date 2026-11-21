---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description: Experience and full CV.
---

[Download the full CV (PDF)](/assets/pdf/cv.pdf){:target="_blank" rel="noopener noreferrer"}

## Experience

{% for job in site.data.experience %}
<div class="row mt-3 mb-4">
  <div class="col-3 col-sm-2">
    {% if job.logo %}<img src="{{ '/assets/img/' | append: job.logo | relative_url }}" alt="{{ job.org }} logo" class="img-fluid" style="background:#fff;padding:4px;border-radius:4px" loading="lazy">{% endif %}
  </div>
  <div class="col-9 col-sm-10">
    <p class="mb-1"><strong>{{ job.role }}</strong> · {{ job.org }} · {{ job.place }}</p>
    <p class="mb-1 text-muted small">{{ job.dates }}</p>
    <p class="mb-0">{{ job.summary }}</p>
  </div>
</div>
{% endfor %}
