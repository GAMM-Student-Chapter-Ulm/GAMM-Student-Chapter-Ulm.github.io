---
title: "GAMM Tagung 2026 in Stuttgart"
date: 2026-03-20
categories:
  - Activities
  - Annual GAMM Meeting
tags:
  - GAMM
  - Tagung
  - Conference
  - Stuttgart
  - Research
author: "Student Chapter Ulm"
excerpt: "96th GAMM Annual Meeting 2026 in Stuttgart"
header:
  teaser: "/assets/images/DSC08513-Poprawione-Szum.jpeg"
  overlay_image: "/assets/images/DSC08513-Poprawione-Szum.jpeg"
  overlay_filter: 0.4
  caption: "Photo: GAMM Tagung 2026, Stuttgart"
---

Seven members of our GAMM/SIAM Student Chapter participated in the GAMM Annual Meeting 2026 in Stuttgart from March 16 to March 20, 2026. 
In addition to many informative and engaging talks, the conference offered our members the opportunity to meet students from other student chapters at various universities and to establish valuable connections.
A special highlight of the meeting was that Carolin Müller, representing our student chapter, together with Prof. Karsten Urban, took part in the handover for the next annual meeting. On this occasion, the key details of the GAMM Annual Meeting 2027 in Ulm were presented. The upcoming meeting will be organized jointly with the German Mathematical Society (DMV) and will take place at Ulm University and Ulm University of Applied Sciences from March 8 to March 12, 2027.

As a GAMM/SIAM Student Chapter, we are very pleased to have the opportunity to help organize the next annual meeting. 
We would like to thank the organizers at the University of Stuttgart for the excellent event.
---

*Want to join us at the next GAMM Tagung? [Become a member](/membership/) of our Student Chapter!*


<div class="slideshow">
  <div class="slides">
    <img src="/assets/images/Stuttgart26_Group.jpg" alt="GAMM Conference in Stuttgart – Group">
    <img src="/assets/images/Stuttgart26_Urban_Mueller.jpg" alt="GAMM Conference in Stuttgart – Invitation to Ulm">
    <img src="/assets/images/Stuttgart26_Urban_Mueller2.jpg" alt="GAMM Conference in Stuttgart – Invitation to Ulm">
  </div>

  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>
  <button class="next" onclick="changeSlide(1)">&#10095;</button>

  <div class="dots">
    <span class="dot" onclick="showSlide(0)"></span>
    <span class="dot" onclick="showSlide(1)"></span>
    <span class="dot" onclick="showSlide(2)"></span>
  </div>
</div>

<style>
.slideshow {
  position: relative;
  max-width: 900px;
  margin: 30px auto;
  overflow: hidden;
  border-radius: 8px;
}

.slides img {
  width: 100%;
  height: 500px;
  object-fit: contain;
  display: none;
}

.slides img.active {
  display: block;
}

.prev,
.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0, 0, 0, 0.5);
  color: white;
  border: none;
  padding: 12px 18px;
  font-size: 24px;
  cursor: pointer;
  border-radius: 4px;
}

.prev {
  left: 15px;
}

.next {
  right: 15px;
}

.dots {
  text-align: center;
  padding: 12px;
}

.dot {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 0 5px;
  background: #bbb;
  border-radius: 50%;
  cursor: pointer;
}

.dot.active {
  background: #333;
}
</style>

<script>
let currentSlide = 0;
const slides = document.querySelectorAll('.slides img');
const dots = document.querySelectorAll('.dot');

function showSlide(index) {
  slides.forEach(slide => slide.classList.remove('active'));
  dots.forEach(dot => dot.classList.remove('active'));

  currentSlide = index;

  slides[currentSlide].classList.add('active');
  dots[currentSlide].classList.add('active');
}

function changeSlide(direction) {
  currentSlide += direction;

  if (currentSlide >= slides.length) {
    currentSlide = 0;
  }

  if (currentSlide < 0) {
    currentSlide = slides.length - 1;
  }

  showSlide(currentSlide);
}

showSlide(0);

setInterval(() => {
  changeSlide(1);
}, 5000);
</script>