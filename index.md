---
layout: splash
---

<!-- 1. The Banner Image -->
<img src="/assets/images/IMG_2856.jpg" alt="Panorama of Ulm" style="width: 100%; max-height: 400px; object-fit: cover; border-radius: 8px; margin-bottom: 2.5em; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">

<!-- 2. The Two-Column Layout -->
<div style="display: flex; flex-wrap: wrap; gap: 3em; text-align: left;">
  
  <!-- Left Column: Main Welcome Text -->
  <div style="flex: 2; min-width: 300px;">
    <h2 style="margin-top: 0;">Welcome to the Student Chapter Ulm!</h2>
    
    <p>We are a group of various Bachelor, Master and PhD students in the field of applied mathematics in Ulm, Germany.</p>
    
    <p>With the beginning of 2019 we formed a GAMM Student Chapter. The <a href="https://www.gamm.org/en/">GAMM</a> (Gesellschaft für Angewandte Mathematik und Mechanik, engl.: Association of Applied Mathematics and Mechanics) is a German society for applied mathematics and mechanics.</p>
    
    <p>Since spring of 2023 we are also a <a href="http://siam.org/">SIAM</a> Student Chapter. The SIAM (Society for Industrial and Applied Mathematics) is also a society for applied mathematics and mechanics, but is based in the U.S. and consists of applied mathematicians and computational scientists worldwide.</p>
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