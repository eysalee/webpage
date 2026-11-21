---
layout: default
title: Service
permalink: /service.html
---

<div class="container mt-3">
      <h2>Service</h2>
        <h4>Program Committees</h4>
        <h5>Conferences</h5>
        <ul>
          {% for c in site.data.committees.conferences %}
          <li>
            {{ c.venue }}{% if c.additional%} ({{ c.additional }}){% endif%}
          </li>
          {% endfor %}
        </ul>
        <h5>Workshops</h5>
        <ul>
          {% for w in site.data.committees.workshops %}
          <li>
            {{ w.venue }}{% if w.additional%} ({{ w.additional }}){% endif%}
          </li>
          {% endfor %}
        <h5>External Reviews</h5>
        <ul>
          <li>2025: CRYPTO</li>
          <li>2024: Eurocrypt</li>
          <li>2023: Eurocrypt, CCS</li>
          <li>2021: CRYPTO</li>
          <li>2020: Eurocrypt, S&P, TCC, CANS, AFT</li>
          <li>2019: Eurocrypt, CRYPTO, TCC, AFT</li>
          <li>2018: CRYPTO</li>
        </ul>
        <h4>Committees</h4>
        <ul>
          {% for c in site.data.committees.committees %}
          <li>
            {{ c.title }} (c.start - c.end)
          </li>
          {% endfor %}
        </ul>
        <h4>Event Organization</h4>
        <ul>
          {% for w in site.data.committees.organizer %}
          <li>
            {{ w.title }}{% if w.additional%} ({{ w.additional }}){% endif%}
          </li>
          {% endfor %}
        </ul>
        <h4>Rump Sessions Chaired</h4>
        <ul>
          <li>CRYPTO 2026</li>
          <li>CRYPTO 2025</li>
          <li>CRYPTO 2024</li>
        </ul>
  </div>