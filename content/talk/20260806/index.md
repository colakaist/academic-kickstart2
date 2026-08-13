---
title: "Farewell Dinner for Our Interns (Aug 2026)"
date: 2026-08-06
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

  <button
    class="farewell-button farewell-prev"
    type="button"
    onclick="changeFarewellImage(-1)"
    aria-label="Previous image">
    &#10094;
  </button>

  <button
    class="farewell-button farewell-next"
    type="button"
    onclick="changeFarewellImage(1)"
    aria-label="Next image">
    &#10095;
  </button>

  <div id="farewell-counter" class="farewell-counter">
    1 / 2
  </div>
</div>

<script>
  const farewellImages = [
    "featured.jpg",
    "2.jpg"
  ];

  let farewellImageIndex = 0;

  function changeFarewellImage(direction) {
    farewellImageIndex =
      (farewellImageIndex + direction + farewellImages.length)
      % farewellImages.length;

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
</script>

<style>
  .farewell-slider {
    position: relative;
    width: 100%;
    max-width: 1120px;
    margin: 20px auto;
    padding: 0 60px;
    box-sizing: border-box;
    background: white;
  }

  .farewell-image {
    display: block;
    width: 100%;
    height: 630px;
    object-fit: contain;
    background: white;
  }

  .farewell-button {
    position: absolute;
    top: 50%;
    z-index: 2;
    transform: translateY(-50%);
    width: 48px;
    height: 60px;
    padding: 0;
    border: none;
    border-radius: 5px;
    color: white;
    background: rgba(0, 0, 0, 0.45);
    font-size: 30px;
    cursor: pointer;
  }

  .farewell-button:hover {
    background: rgba(0, 0, 0, 0.75);
  }

  .farewell-prev {
    left: 6px;
  }

  .farewell-next {
    right: 6px;
  }

  .farewell-counter {
    position: absolute;
    right: 72px;
    bottom: 10px;
    padding: 4px 10px;
    border-radius: 4px;
    color: white;
    background: rgba(0, 0, 0, 0.55);
    font-size: 14px;
  }

  @media (max-width: 700px) {
    .farewell-slider {
      padding: 0 45px;
    }

    .farewell-image {
      height: 350px;
    }

    .farewell-button {
      width: 36px;
      height: 48px;
      font-size: 22px;
    }

    .farewell-prev {
      left: 4px;
    }

    .farewell-next {
      right: 4px;
    }

    .farewell-counter {
      right: 55px;
    }
  }
</style>
