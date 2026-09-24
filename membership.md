---
layout: splash
title: "Membership"
permalink: /membership/
author_profile: false
---

<!-- 1. The Banner Image -->
<img src="/assets/images/IMG_2856_compressed.webp" alt="Panorama of Ulm" style="width: 100%; max-height: 400px; object-fit: cover; border-radius: 8px; margin-bottom: 2.5em; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">

<!-- 2. The Two-Column Layout -->
<div style="display: flex; flex-wrap: wrap; gap: 3em; text-align: left;">
  
  <!-- Left Column: Main Content -->
  <div style="flex: 2; min-width: 300px;">
    <h2 style="margin-top: 0;">Membership</h2>
    
    <p>Being a member of the Student Chapter Ulm has many benefits. To get this honor, you just need to fill out the <a href="#">registration form</a>.</p>
    
    <p>Thereby you will be recognized as a member of our Student Chapter and will be added to our mailing list. Please use your <code>@uni-ulm.de</code> or <code>@thu.de</code> mail address, so that we can verify that you are part of one of these institutions.</p>
    
    <p>Since we are a simultaneous Student Chapter of GAMM and SIAM, you can become a member of either one, but ideally of both of these institutions.</p>
    
    <h3>GAMM Membership</h3>
    <p>For the GAMM membership we will forward your contact data and you will automatically become a student member of the GAMM (Gesellschaft für Angewandte Mathematik und Mechanik).</p>
    
    <h3>SIAM Membership</h3>
    <p>To become a student member of the SIAM (Society for Industrial and Applied Mathematics) you will need to sign up yourself <a href="https://my.siam.org/" target="_blank" rel="noopener noreferrer">here</a>. Just select the free undergraduate or graduate (whichever applies to you) student tier and register. During the process make sure to choose the <strong>Ulm Student Chapter</strong> from the list.</p>
    
    <p><strong>The best news for you:</strong> the GAMM and (student) SIAM membership is <strong>free of charge for an unlimited period</strong> as long as you maintain your student status (undergraduate or PhD).</p>
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