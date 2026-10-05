---
title: "Meeting the Augsburg Student Chapter"
categories:
  - Activities
---
On June 25, 2026, a group of three GAMM members from Ulm visited the GAMM Student Chapter Group in Augsburg.

The meeting provided a great opportunity for scientific exchange, interesting discussions, and getting to know each other better over a shared lunch. We also agreed to stay in close contact, continue exchanging ideas, and plan joint activities in the future.

A big thank you to the Augsburg group for the kind invitation and the warm welcome! We are already looking forward to the next meeting and to many more opportunities for collaboration and exchange.

<div class="slideshow">
  <div class="slides">
    <img src="/assets/images/Ausgburg_2026JAGUARS_feat.Ulm_Jun26.jpg" alt="Meeting in Augsburg 2026">
  </div>

  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>
  <button class="next" onclick="changeSlide(1)">&#10095;</button>

  <div class="dots">
    <span class="dot" onclick="showSlide(0)"></span>
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