---
layout: page
title: BIOS740
nav_exclude: true
permalink: /:path/
seo:
  type: Course
  name: BIOS740
---
# Welcome to BIOS740

{% assign announcements = site.announcements | sort: "date" | reverse %}
{% for announcement in announcements limit:5 %}
  <div class="announcement">
    <h3>{{ announcement.title }}</h3>
    <small>{{ announcement.date | date: "%B %-d, %Y" }}</small>
    <div>{{ announcement.content | markdownify }}</div>
  </div>
{% endfor %}


<div style="
  max-width: 700px;
  margin: 2.5em auto;
  padding: 2em 1.5em 1.5em 1.5em;
  background: #f6faff;
  border-radius: 2em;
  box-shadow: 0 6px 32px rgba(50,75,170,0.10);
  text-align: center;
  border: 1.5px solid #dde3ee;
">
  <h2 style="margin-top: 0; font-family: inherit; font-size: 2.2em; color: #304065; letter-spacing: 0.02em;">
    🌍 Global Visitor Map
  </h2>
  <div style="margin-bottom: 1.5em; color: #607088; font-size: 1.25em;">
    See where in the world our website is making an impact! The interactive map below shows the locations of recent visitors.
  </div>
  <div style="display: flex; justify-content: center;">
    <div style="width: 550px; max-width: 100%;">
      <script type="text/javascript" id="clustrmaps" src="https://clustrmaps.com/map_v2.js?d=ALDrEcc70EcnoYv3VnXoQ6s_bSg8_DAaAU7G_5JOPlI&cl=ffffff&w=a"></script>
    </div>
  </div>
  <div style="margin-top: 1.5em; color: #a8adc0; font-size: 1.05em;">
    Powered by <a href="https://clustrmaps.com/" target="_blank" style="color:#4777e4;text-decoration:underline;">ClustrMaps</a>
  </div>
</div>



