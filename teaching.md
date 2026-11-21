---
layout: default
title: Teaching
permalink: teaching.html
---

<div class="container mt-3">
      <h2>Courses</h2>
      {% if site.data.courses.upcoming.semester %}
      <h5>Upcoming</h5>
      <ul>
        {% for offering in site.data.courses.upcoming.offerings %}
        <li>{{ site.data.courses.upcoming.semester }}: <a href="{{ offering.url }}">{{ offering.course_number }}</a> ({{ offering.title }})</li>
        {% endfor %}
      </ul>
      {% endif %}
      <h5>Current</h5>
      <ul>
        {% for offering in site.data.courses.current.offerings %}
        <li>{{ site.data.courses.current.semester }}: <a href="{{ offering.url }}">{{ offering.course_number }}</a> ({{ offering.title }})</li>
        {% endfor %}
      </ul>
        <h5>Previous</h5>
      <ul>
        {% for offering in site.data.courses.previous %}
        <li>{{ offering.course_number }} ({{ offering.title }}): 
        {% for iter in offering.iterations %}
        {% unless forloop.first %}, {% endunless %}
        <a href="{{ iter.url }}">{{ iter.semester }}</a>
        {% endfor %}
        </li>
        {% endfor %}
        </ul>
    <!-- </div>
    <div class="container mt-3"> -->
      <br>
      <h2>Students</h2>
      I'm very happy to have had the opportunity to work with students on research projects while at Barnard. Students I've supervised include:
      <ul>
        <li>Undergraduate Students:
          <ul>
            <!-- <li>Harita Suresh (Barnard), Spring 2027 - Present</li> -->
            <li>Ruby Chang (Columbia), Fall 2025 - Present</li>
            <li>Tony Fields (Columbia), Fall 2025 - Present</li>
            <li>Rohan Jangama (UT Austin), Summer 2026 (Visiting Student)</li>
            <li>Trish Nguyen (Barnard), Summer 2026 (SRI)</li>
            <li>Elizabeth Wei (NYU), Summer 2025 (Cyber NYC REU)</li>
          </ul>
        </li>
        <li>Master's Students:
          <ul>
            <li>Giancarlo Pacenza (Columbia), Summer 2026 - Present</li>
          </ul>
        </li>
      </ul>
      If you would like to work with me, please see this <a href="workwithme.html">page</a> for more information.
  </div>