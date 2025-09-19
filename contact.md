---
layout: default
title: Contact
---

<div class="max-w-4xl mx-auto prose prose-lg">
  <h1 class="text-3xl font-bold text-green-800 mb-6">Contact Us</h1>

  {% for office in site.conference.offices %}
  <section class="mb-8">
    <h2 class="text-2xl font-bold mb-4">{{ office.name }}</h2>
    <p><strong>{{ office.org }}</strong></p>
    <p>{{ office.address }}</p>
    <p><strong>Phone:</strong> {{ office.phone }} ({{ office.contact }})</p>
  </section>
  {% endfor %}

  <p class="mt-8"><strong>Website:</strong> <a href="{{ site.conference.website }}">{{ site.conference.website }}</a> | <strong>Email:</strong> <a href="mailto:{{ site.conference.email }}">{{ site.conference.email }}</a></p>

  <p>For paper submissions and inquiries, please contact the offices above.</p>
</div>