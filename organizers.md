---
layout: default
title: Organizers
---

<div class="py-8 max-w-4xl mx-auto">
  <h1 class="text-3xl font-bold text-green-800 mb-8 text-center">Our Esteemed Team</h1>

  <section class="mb-12">
    <h2 class="text-2xl font-bold text-green-700 mb-6">Patrons</h2>
    <div class="grid md:grid-cols-3 gap-6">
      {% for patron in site.conference.patrons %}
      <div class="bg-white p-6 rounded-lg shadow-md text-center">
        {% if patron.image %}
        <img src="{{ patron.image }}" alt="{{ patron.name }}" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover">
        {% endif %}
        <h3 class="text-xl font-semibold text-green-700 mb-2">{{ patron.name }}</h3>
        <p class="text-gray-600 italic">{{ patron.title }}</p>
      </div>
      {% endfor %}
    </div>
  </section>

  <section class="mb-12">
    <h2 class="text-2xl font-bold text-green-700 mb-6">Convenors</h2>
    <div class="grid md:grid-cols-3 gap-6">
      {% for convener in site.conference.convenors %}
      <div class="bg-white p-6 rounded-lg shadow-md text-center">
        {% if convener.image %}
        <img src="{{ convener.image }}" alt="{{ convener.name }}" class="w-24 h-24 rounded-full mx-auto mb-4 object-cover">
        {% endif %}
        <h3 class="text-xl font-semibold text-green-700 mb-2">{{ convener.name }}</h3>
        <p class="text-gray-600 italic">{{ convener.title }}</p>
      </div>
      {% endfor %}
    </div>
  </section>

  <section>
    <h2 class="text-2xl font-bold text-green-700 mb-6">Organizers</h2>
    <div class="bg-green-100 p-6 rounded-lg">
      <ul class="list-disc list-inside space-y-2 text-lg">
        {% for org in site.conference.organizers %}
        <li>{{ org }}</li>
        {% endfor %}
      </ul>
    </div>
  </section>
</div>