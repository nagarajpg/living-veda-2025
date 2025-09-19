---
layout: default
title: Call for Papers
---

<div class="prose prose-lg max-w-none">
  <h1 class="text-3xl font-bold text-green-800 mb-6">Call for Papers</h1>

  <p>Scholars, researchers, and practitioners are invited to submit papers that explore the contemporary relevance of the Veda in its many dimensions.</p>

  <h2 class="text-2xl font-bold mt-8 mb-4">Suggested Topics</h2>
  <ul class="list-disc pl-6 space-y-2">
    {% for topic in site.conference.call_for_papers.topics %}
    <li>{{ topic }}</li>
    {% endfor %}
  </ul>

  <h2 class="text-2xl font-bold mt-8 mb-4">Submission Guidelines</h2>
  <ul class="list-disc pl-6 space-y-2">
    {% for guideline in site.conference.call_for_papers.guidelines %}
    <li>{{ guideline }}</li>
    {% endfor %}
  </ul>

  <h2 class="text-2xl font-bold mt-8 mb-4">Benefits of Participation</h2>
  <ul class="list-disc pl-6 space-y-2">
    {% for benefit in site.conference.call_for_papers.benefits %}
    <li>{{ benefit }}</li>
    {% endfor %}
  </ul>

  <div class="text-center mt-8">
    <a href="{{ site.baseurl }}/contact