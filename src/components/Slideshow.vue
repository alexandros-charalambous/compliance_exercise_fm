<template>
  <section class="content">
    <div class="slideshow1">
      <img src="@/assets/slideshow1.png" alt="Slideshow1" />
    </div>
    <div class="slideshow2">
      <img src="@/assets/slideshow2.png" alt="Slideshow2" />
    </div>
    <div class="slideshow3">
      <img src="@/assets/slideshow3.png" alt="Slideshow3" />
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.content {
  overflow: hidden;
  height: 400px;
  display: flex;
  justify-content: center;
  @media (max-width: 1439px) {
    justify-content: left;
  }
}

.content div {
  width: 500px;
  align-content: center;
}

.slideshow1 {
  background: radial-gradient(
      50% 50% at 50% 100%,
      var(--color-alt) 0%,
      rgba(19, 53, 245, 0.33) 50%,
      rgba(19, 53, 245, 0) 100%
    ),
    linear-gradient(360deg, var(--color-alt) -100%, rgba(19, 53, 245, 0) 100%),
    linear-gradient(0deg, #000000, #000000);
}

.slideshow2 {
  background: radial-gradient(
    50% 50% at 50% 100%,
    var(--color-alt) 0%,
    rgba(19, 53, 245, 0.33) 50%,
    rgba(19, 53, 245, 0) 100%
  );
}

.slideshow2 img {
  transform: rotateX(3.02deg);
}

.slideshow3 {
  background: radial-gradient(
      50% 50% at 50% 100%,
      var(--color-alt) 0%,
      rgba(19, 53, 245, 0.33) 50%,
      rgba(19, 53, 245, 0) 100%
    ),
    linear-gradient(360deg, var(--color-alt) -100%, rgba(19, 53, 245, 0) 100%),
    linear-gradient(0deg, #000000, #000000);
}
</style>
