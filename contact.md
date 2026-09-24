---
layout: splash
title: "Contact"
permalink: /contact/
author_profile: false
---

<!-- 1. The Banner Image -->
<img src="/assets/images/IMG_2856_compressed.webp" alt="Panorama of Ulm" style="width: 100%; max-height: 400px; object-fit: cover; border-radius: 8px; margin-bottom: 2.5em; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">

<!-- 2. The Two-Column Layout -->
<div style="display: flex; flex-wrap: wrap; gap: 3em; text-align: left;">
  
  <!-- Left Column: Main Content -->
  <div style="flex: 2; min-width: 300px;">
    <h2 style="margin-top: 0;">Contact Us</h2>
    
    <p>We are always happy to hear from fellow students, researchers, or anyone interested in applied mathematics and mechanics!</p>
    
    <h3>General Inquiries</h3>
    <p>For general requests, questions about membership, or upcoming events, please write us an email at:</p>
    <p>📧 <strong><a href="mailto:contact@studentchapter-ulm.de">contact@studentchapter-ulm.de</a></strong></p>
    
    <h3>Website & GitHub</h3>
    <p>Did you find a typo, a broken link, or want to suggest an improvement for this website?</p>
    <p>Because our website is completely open-source, you can directly open an issue or a Pull Request on our <a href="https://github.com/GAMM-Student-Chapter-Ulm/GAMM-Student-Chapter-Ulm.github.io" target="_blank" rel="noopener noreferrer">GitHub Repository</a>. Alternatively, you can reach out to our webmaster via the general email address above.</p>
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

---

**Legal Information**  
Please see our [Impressum](/impressum/) and [Datenschutzerklärung](/datenschutz/) for further legal and privacy details.