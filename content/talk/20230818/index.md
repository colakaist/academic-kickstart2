---
title: "Seungho's Talk @ ICBP2023 (Aug 2023)"
date: "2023-08-18"
showDate: true

image:
  preview_only: true
---


<!--more-->

<div class="farewell-slider">
  <img
    id="farewell-image"
    class="farewell-image"
    src="featured.jpg"
    alt="Farewell dinner photo 1"
  >

  <div
    id="farewell-counter"
    class="farewell-counter">
    1 / 8
  </div>
</div>

<script>
  const farewellImages = [
    "featured.jpg",
    "2.jpg",
    "3.jpg",
    "4.jpg",
    "5.jpg",
    "6.jpg",
    "7.jpg",
    "8.jpg"
  ];

  let farewellImageIndex = 0;

  function showNextFarewellImage() {
    farewellImageIndex =
      (farewellImageIndex + 1) % farewellImages.length;

    const image =
      document.getElementById("farewell-image");

    const counter =
      document.getElementById("farewell-counter");

    image.src =
      farewellImages[farewellImageIndex];

    image.alt =
      "Farewell dinner photo " + (farewellImageIndex + 1);

    counter.textContent =
      (farewellImageIndex + 1) +
      " / " +
      farewellImages.length;
  }

  setInterval(showNextFarewellImage, 1000);
</script>

<style>
  .farewell-slider {
    position: relative;
    width: 100%;
    max-width: 1000px;
    margin: 20px auto;
    overflow: hidden;
    background: white;
  }

  .farewell-image {
    display: block;
    width: 100%;
    height: 630px;
    object-fit: contain;
    background: white;
    transition: opacity 0.5s ease-in-out;
  }

  .farewell-counter {
    position: absolute;
    right: 12px;
    bottom: 10px;
    padding: 4px 10px;
    border-radius: 4px;
    color: white;
    background: rgba(0, 0, 0, 0.55);
    font-size: 14px;
  }

  @media (max-width: 700px) {
    .farewell-image {
      height: 350px;
    }
  }
</style>











