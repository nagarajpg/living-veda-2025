---
layout: home
title: Home
---

<div class="py-8">
  <div class="text-center mb-8">
    <h1 class="text-4xl font-bold text-green-800 mb-2">{{ site.conference.name }}</h1>
    <h2 class="text-2xl mb-6">{{ site.conference.full_name }}</h2>
  </div>

  <div class="flex flex-col md:flex-row justify-center items-center space-y-4 md:space-y-0 md:space-x-8 mb-8">
    <div class="text-center">
      <span class="text-4xl">📅</span>
      <p class="font-bold">{{ site.conference.dates }}</p>
    </div>
    <div class="text-center">
      <span class="text-4xl">🏛️</span>
      <p class="font-bold">{{ site.conference.location }}</p>
      <p>{{ site.conference.address }}</p>
    </div>
  </div>

  <div class="grid md:grid-cols-2 gap-6 mb-8 max-w-4xl mx-auto">
    {% for office in site.conference.offices %}
    <div class="bg-white p-6 rounded-lg shadow-md">
      <h3 class="font-bold text-green-700 mb-2">{{ office.name }}</h3>
      <p><strong>{{ office.org }}</strong></p>
      <p>{{ office.address }}</p>
      <p><strong>Phone:</strong> {{ office.phone }} ({{ office.contact }})</p>
    </div>
    {% endfor %}
  </div>

  <div class="flex justify-center space-x-6 mb-8">
    <img src="{{ site.conference.logos.central_sanskrit }}" alt="Central Sanskrit University" class="w-20 h-auto">
    <img src="{{ site.conference.logos.sanskriti }}" alt="Sanskriti University" class="w-20 h-auto">
    <img src="{{ site.conference.logos.sri_aurobindo_society }}" alt="Sri Aurobindo Society" class="w-20 h-auto">
    <img src="{{ site.conference.logos.sakshi_trust }}" alt="SAKSHI Trust" class="w-20 h-auto">
  </div>

  <div class="text-center">
    <a href="/theme-note" class="btn mr-4">Theme Note</a>
    <a href="/call-for-papers" class="btn mr-4">Call for Papers</a>
    <a href="{{ site.conference.registration_link }}" target="_blank" class="btn">Register</a>
  </div>
</div>