---
layout: default
title: Research
permalink: /research.html
---

<div class="container mt-3">
  <div class="row">
    <div id="Research" class="col-12">
      <h2>Research</h2>
      My research interests are in cryptography, and specifically signatures and multi-party computation.
      <br>
      Recently I've been interested in policy (see <a href="https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework/issues/200" target="_blank">Cryptographers’ Feedback on the EU Digital Identity’s ARF</a>)--I hope to have more updates in the future!
      <br>
      <br>
      <h5>Threshold ECDSA</h5>
      For information about the "DKLs" threshold ECDSA signing schemes, we have a <a href="https://dkls.info/" target="_blank">website</a>! We always love hearing from people who have deployed or used our schemes... Please feel free to reach out if you know of any implementations we've missed! :)
    </div>
    <div class="col-12">
      <div class="row mt-3">
        <div class="col">
          <h3>Papers</h3>
          <p class="text-muted">Authors are listed in alphabetical order, unless otherwise specified.<p>
        <!-- <h5>Preprints</h5>
        <ul>
        </ul> -->
    <div class="col-12">
      <div class="row mt-2">
        <div class="col">
          <h5>Conference Publications</h5>
          <ul>
            {% for paper in site.data.publications.conference %}
            <li>
              {{ paper.title }}
              <br>
              {{ paper.authors }}
              <br>
              {{ paper.venue }}
              <br>
              {% if paper.paper_link %}[<a href="{{ paper.paper_link }}" target="_blank">Paper</a>]{% endif %} 
              {% if paper.code_link %}[<a href="{{ paper.code_link }}" target="_blank">Code</a>]{% endif %} 
              {% if paper.slides_link %}[<a href="{{ paper.slides_link }}" target="_blank">Slides</a>]{% endif %}
            </li>
            {% endfor %}
          </ul>
        </div>
      </div>
    </div>
    <div class="col-12">
      <div class="row mt-2">
      <div class="col-12">
        <h5>Journal Publications</h5>
        <ul>
            {% for paper in site.data.publications.journal %}
            <li>
              {{ paper.title }}
              <br>
              {{ paper.authors }}
              <br>
              {{ paper.venue }}
              <br>
              {% if paper.paper_link %}[<a href="{{ paper.paper_link }}" target="_blank">Paper</a>]{% endif %} 
              {% if paper.code_link %}[<a href="{{ paper.code_link }}" target="_blank">Code</a>]{% endif %} 
              {% if paper.slides_link %}[<a href="{{ paper.slides_link }}" target="_blank">[lides</a>]{% endif %}
            </li>
            {% endfor %}
          </ul>
      </div>
      </div>
    </div>
    <div class="col-12">
      <div class="row mt-3">
        <div class="col">
          <h3>Workshop Contributions</h3>
          <h5>Talks</h5>
          <ul>
            {% for talk in site.data.publications.workshop_talks %}
            <li>
              {{ talk.title }}
              <br>
              Speakers: {{ talk.speakers }}
              <br>
              {{ talk.venue }}
              <br>
              {% if talk.abstract %}[<a href="{{ talk.abstract }}" target="_blank">Abstract</a>]{% endif %} 
              {% if talk.slides_link %}[<a href="{{ talk.slides_link }}" target="_blank">Slides</a>]{% endif %}
            </li>
            {% endfor %}
          </ul>
        <h5>Misc</h5>
          <ul>
            {% for misc in site.data.publications.misc_contributions %}
            <li>
              {{ misc.title }}
              <br>
              {{ misc.author }}
              <br>
              {{ misc.venue }}
              <br>
              [<a href="{{ misc.artifact }}">Artifact</a>]
            </li>
            {% endfor %}
          </ul>
      </div>
  </div>
</div>