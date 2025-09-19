---
layout: home
title: Home
---

<div class="text-center py-8 bg-green-50">
  <div class="flex justify-center items-center mb-6 flex-col md:flex-row">
    <img src="{{ site.baseurl }}/assets/images/living-veda-logo.png" alt="Living Veda Logo" class="w-24 h-auto mb-4 md:mb-0 md:mr-4">
    <div>
      <h1 class="text-4xl font-bold text-green-800 sm:text-3xl">{{ site.conference.name }}</h1>
      <h2 class="text-xl sm:text-lg">{{ site.conference.full_name }}</h2>
    </div>
  </div>
  
  <div class="bg-white p-6 rounded-lg shadow-md inline-block mb-8 w-full md:w-auto">
    <div class="flex justify-center items-center mb-4 flex-col sm:flex-row">
      <img src="{{ site.baseurl }}/assets/images/calendar-icon.png" alt="Calendar" class="w-8 h-8 mr-0 sm:mr-2 mb-2 sm:mb-0">
      <strong>{{ site.conference.dates }}</strong>
    </div>
    <div class="flex justify-center items-center flex-col sm:flex-row">
      <img src="{{ site.baseurl }}/assets/images/location-icon.png" alt="Location" class="w-8 h-8 mr-0 sm:mr-2 mb-2 sm:mb-0">
      <strong>{{ site.conference.location }}</strong><br class="sm:hidden">{{ site.conference.address }}
    </div>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8 max-w-4xl mx-auto">
    {% for office in site.conference.offices %}
    <div class="bg-white p-4 rounded-lg shadow-md">
      <h3 class="font-bold text-green-700 text-lg sm:text-xl">{{ office.name }}</h3>
      <p><strong>{{ office.org }}</strong></p>
      <p class="text-sm sm:text-base">{{ office.address }}</p>
      <p><strong>Phone:</strong> {{ office.phone }}<br><em>{{ office.contact }}</em></p>
    </div>
    {% endfor %}
  </div>

  <div class="flex justify-center space-x-6 mb-8 flex-wrap">
    <img src="{{ site.baseurl }}/assets/images/central-sanskrit-uni-logo.png" alt="Central Sanskrit University Logo" class="w-20 h-auto mb-4 sm:mb-0">
    <img src="{{ site.baseurl }}/assets/images/sanskriti-uni-logo.png" alt="Sanskriti University Logo" class="w-20 h-auto mb-4 sm:mb-0">
    <img src="{{ site.baseurl }}/assets/images/sri-aurobindo-society-logo.png" alt="Sri Aurobindo Society Logo" class="w-20 h-auto mb-4 sm:mb-0">
    <img src="{{ site.baseurl }}/assets/images/sakshi-trust-logo.png" alt="SAKSHI Trust Logo" class="w-20 h-auto mb-4 sm:mb-0">
  </div>

  <!-- Highlighted Action Section -->
  <div class="mb-8">
    <h3 class="text-2xl font-bold text-green-800 mb-6 text-center">Get Involved</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-4xl mx-auto">
      <a href="{{ site.baseurl }}/theme-note" class="btn-highlight-large orange w-full">
        <div class="text-center">
          <span class="text-3xl mb-2">📖</span>
          <h4 class="text-xl font-bold mb-2">Theme Note</h4>
          <p class="text-sm text-gray-700">Explore the vision</p>
        </div>
      </a>
      <a href="{{ site.baseurl }}/call-for-papers" class="btn-highlight-large orange w-full">
        <div class="text-center">
          <span class="text-3xl mb-2">✍️</span>
          <h4 class="text-xl font-bold mb-2">Call for Papers</h4>
          <p class="text-sm text-gray-700">Submit your abstract</p>
        </div>
      </a>
      <a href="{{ site.conference.registration_link }}" target="_blank" class="btn-highlight-large green w-full">
        <div class="text-center">
          <span class="text-3xl mb-2">📝</span>
          <h4 class="text-xl font-bold mb-2">Register</h4>
          <p class="text-sm text-gray-700">Secure your spot</p>
        </div>
      </a>
    </div>
  </div>

  <p class="text-center text-sm text-gray-600 mt-4">Optimized for mobile viewing. Scan the QR code below!</p>
  <img src="{{ site.baseurl }}/assets/images/qr-code.png" alt="QR Code for livingveda.info" class="mx-auto mt-2 w-24 h-24 sm:w-32 sm:h-32">
</div>