---
title: "Langer Abend der Wissenschaft 2022"
categories:
  - Acitivities
---
At the “Langer Abend der Wissenschaft” on July 15, 2022 at Ulm University, the GAMM Student Chapter supported the booth of the Numerics Institute. Visitors could marvel at the double pendulum of the UZWR in experiment as well as in simulation. Furthermore, prospective students could inform themselves about the study program CSE at Ulm University.

<div class="slideshow">
  <div class="slides">
    <img src="/assets/images/Langer_Abend_der_Wissenschaft/Reinhold_Urban.jpeg" alt="Langer Abend der Wissenschaft 2022">
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