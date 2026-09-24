---
layout: splash
title: "Activities"
permalink: /activities/
author_profile: false
---

<!-- 1. The Banner Image -->
<img src="/assets/images/IMG_2856_compressed.webp" alt="Panorama of Ulm" style="width: 100%; max-height: 400px; object-fit: cover; border-radius: 8px; margin-bottom: 2.5em; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">

<!-- 2. The Two-Column Layout -->
<div style="display: flex; flex-wrap: wrap; gap: 3em; text-align: left;">
  
  <!-- Left Column: All Posts -->
  <div style="flex: 2; min-width: 300px;">
    <h2 style="margin-top: 0;">All Activities & Posts</h2>
    
    <ul style="list-style-type: none; padding-left: 0; margin-bottom: 0;">
      
      {% for post in site.posts %}
        <li style="margin-bottom: 24px; padding-bottom: 24px; border-bottom: 1px solid #eee;">
          <a href="{{ post.url }}" style="text-decoration: none; font-weight: bold; color: #36688d; font-size: 1.2em;">{{ post.title }}</a><br>
          <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small>
          <p style="margin-top: 8px; color: #444;">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        </li>
      {% endfor %}
      
    </ul>
  </div>

  <!-- Right Column: Recent Posts Sidebar -->
  <div style="flex: 1; min-width: 250px; background: #f3f4ef; padding: 1.5em; border-radius: 8px; height: fit-content;">
    <h3 style="margin-top: 0; color: #36688d;">Recent Posts</h3>
    <ul style="list-style-type: none; padding-left: 0; margin-bottom: 0;">
      
      {% for post in site.posts limit:5 %}
        <li style="margin-bottom: 12px;">
          <a href="{{ post.url }}" style="text-decoration: none; font-weight: bold; color: #36688d;">{{ post.title }}</a><br>
          <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small>
        </li>
      {% endfor %}
      
    </ul>
  </div>

</div>