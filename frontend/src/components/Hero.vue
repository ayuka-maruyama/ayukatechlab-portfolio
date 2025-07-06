<!-- HTML部分 -->
<template>
  <section class="hero">
    <div class="overlay top">
      <p class="hero-title">エンジニアも、デザインも、ＡＩも。</p>
    </div>
    <div class="overlay middle">
      <p class="hero-title">得意を生かして、限界に挑戦中！</p>
    </div>
    <div class="overlay bottom">
      <p class="hero-title">だれかの「困った」を、私の「得意」でそっと支える仕事がしたい。</p>
    </div>
  </section>
</template>

<!-- CSS部分 -->
<style scoped>
.hero {
  position: relative;
  width: 100%;
  height: 70vh;
  background: url('@/assets/hero.jpg') top/cover no-repeat;
  background-color: #000;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  margin-top: 20px;
}

.overlay {
  position: absolute;
  background-color: rgba(0, 0, 0, 0.5);
  padding: 1.5rem;
  border-radius: 0.5rem;
}

.top {
  top: 15%;
  left: 5%;
}

.middle {
  top: 40%;
  left: 20%;
}

.bottom {
  bottom: 10%;
  right: 5%;
}

.hero-title {
  font-size: 2rem;
  text-align: center;
  font-weight: bold;
  line-height: 1.4;
}

.overlay.bottom .hero-title {
  font-size: 1rem;
}
</style>
