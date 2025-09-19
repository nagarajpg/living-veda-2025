---
layout: default
title: Call for Papers
---

<div class="bg-orange-50 py-12">
  <div class="container mx-auto px-4 max-w-4xl">
    <!-- Header Section -->
    <h1 class="text-4xl font-bold text-green-800 text-center mb-8 sm:text-3xl md:text-4xl">Call for Papers</h1>

    <!-- Introduction Section -->
    <section class="bg-white rounded-lg shadow-md p-6 mb-8">
      <p class="text-lg leading-relaxed text-left sm:text-base md:text-lg">
        Scholars, researchers, and practitioners are invited to submit papers that explore the contemporary relevance of the Veda in its many dimensions. This conference seeks to illuminate the Veda’s transformative potential in areas such as sustainability, education, governance, and spiritual growth, guided by the insights of Sri Aurobindo.
      </p>
    </section>

    <!-- Suggested Topics Section -->
    <section class="bg-white rounded-lg shadow-md p-6 mb-8">
      <h2 class="text-2xl font-semibold text-orange-700 mb-4 sm:text-xl md:text-2xl">Suggested Topics</h2>
      <ul class="list-disc pl-6 space-y-2 text-lg sm:text-base md:text-lg">
        {% for topic in site.conference.call_for_papers.topics %}
        <li class="leading-relaxed">{{ topic }}</li>
        {% endfor %}
      </ul>
    </section>

    <!-- Submission Guidelines Section -->
    <section class="bg-white rounded-lg shadow-md p-6 mb-8">
      <h2 class="text-2xl font-semibold text-orange-700 mb-4 sm:text-xl md:text-2xl">Submission Guidelines</h2>
      <ul class="list-disc pl-6 space-y-2 text-lg sm:text-base md:text-lg">
        {% for guideline in site.conference.call_for_papers.guidelines %}
        <li class="leading-relaxed">{{ guideline }}</li>
        {% endfor %}
      </ul>
      <p class="text-lg leading-relaxed mt-4 sm:text-base md:text-lg">
        Deadlines: Abstracts by <strong>30th September 2025</strong>, full papers by <strong>30th October 2025</strong>.
      </p>
    </section>

    <!-- Benefits of Participation Section -->
    <section class="bg-white rounded-lg shadow-md p-6 mb-8">
      <h2 class="text-2xl font-semibold text-orange-700 mb-4 sm:text-xl md:text-2xl">Benefits of Participation</h2>
      <ul class="list-disc pl-6 space-y-2 text-lg sm:text-base md:text-lg">
        {% for benefit in site.conference.call_for_papers.benefits %}
        <li class="leading-relaxed">{{ benefit }}</li>
        {% endfor %}
      </ul>
    </section>

    <!-- Submission Action Section -->
    <section class="bg-white rounded-lg shadow-md p-6 text-center">
      <h2 class="text-2xl font-semibold text-orange-700 mb-4 sm:text-xl md:text-2xl">Submit Your Work</h2>
      <button class="btn btn-highlight w-full sm:w-auto mb-2 sm:mb-0" onclick="window.location.href='{{ site.baseurl }}/contact'">Submit Abstract</button>
      <p class="text-sm text-gray-600 mt-2">For inquiries, contact us at <a href="mailto:{{ site.conference.email }}" class="text-orange-600 hover:underline">{{ site.conference.email }}</a>.</p>
    </section>

    <!-- Sri Aurobindo Image -->
    <div class="flex justify-end mt-8">
      {% if site.conference.sri_aurobindo_image %}
      <img src="{{ site.conference.sri_aurobindo_image }}" alt="Sri Aurobindo Portrait" class="w-48 h-auto rounded-full shadow-md">
      {% endif %}
    </div>
  </div>
</div>