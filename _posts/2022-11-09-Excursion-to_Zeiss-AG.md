---
title: "Excursion to ZEISS AG"
categories:
  - Acitivities
  - Excursion
---
On October 27, 2022, the first company excursion of the GAMM Student Chapter Ulm took place. With a total of 16 participants, we started at 8 a.m. from Ulm with an organized bus in the direction of Oberkochen to the headquarters of ZEISS.

After a nice welcome by our excursion supervisor from ZEISS and a first coffee break, the technical part of the day began. A Meditec employee presented the simulation of a tool for inserting an artificial eye lens. We then went together to the ZEISS Medical Solution Center, where various optical devices used in medical practices and surgery are on display. A former employee passionately told us some details and background information about these ZEISS products.
After lunch together, another technical lecture followed. A ZEISS employee, himself a mathematician, gave us some insights into the world of mathematics at ZEISS. He told us where mathematicians are employed at ZEISS. In the course of this, he also introduced us to the project he is currently working on. After this very informative talk, we drove together to the ZEISS Museum, which is also located in Oberkochen. There, the same employee who had already guided us through the Medical Solution Center gave us further insights into the history of ZEISS. After this last program item of the day, we started our way home around 3:30 p.m.

A big thank you goes to the Carl ZEISS AG for their hospitality and the opportunity to get so many interesting impressions into the world of optics. The whole day was very well organised. Another thank you goes to the project InnoTEACH, who provided the financial means for the bus and made it possible that we could carry out the excursion without additional costs for the participants.

Thanks as well to all participants for the nice day together. We are very much looking forward to having you with us again at our next excursion.

<div class="slideshow">
  <div class="slides">
    <img src="/assets/images/Zeiss_2022/Zeiss_1.jpg" alt="Excursion to ZEISS AG">
    <img src="/assets/images/Zeiss_2022/Zeiss_2.jpg" alt="Excursion to ZEISS AG">
    <img src="/assets/images/Zeiss_2022/Zeiss_3.jpg" alt="Excursion to ZEISS AG">
    <img src="/assets/images/Zeiss_2022/Zeiss_4.jpeg" alt="Excursion to ZEISS AG">
    <img src="/assets/images/Zeiss_2022/Zeiss_5.jpeg" alt="Excursion to ZEISS AG">
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