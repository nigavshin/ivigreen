<script setup>
import BaseButton from "./ui/BaseButton.vue";
</script>
<template>
  <main class="main">
    <div class="main__container container">
      <article class="main__content">
        <h2 class="main__content-title">
          Social-Emotional Learning Toolkits and Soft Skills for Educators
        </h2>
        <p class="main__content-text">
          Fostering emotional intelligence and progressive mindset in teen
          students
        </p>
        <BaseButton label="Show all kits" />
      </article>
      <article class="main__picture">
        <img
          class="main__picture-img"
          src="../assets/main-picture.png"
          width="600"
          height="600"
          alt="peoples read books"
        />
        <p class="main__picture-text main__picture-text--first">
          Engaging activities for classroom and home use
        </p>
        <p class="main__picture-text main__picture-text--second">
          Comprehensive guidelines for educators
        </p>
        <p class="main__picture-text main__picture-text--third">
          Ready-to-use materials for SEL classes
        </p>
      </article>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.main {
  padding: 34px 0;
  background-color: var(--general);
}

.main__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 90px;
}

.main__content {
  color: var(--text-light);
}

.main__content-title {
  margin: 0 0 20px;
  font-size: 40px;
  font-weight: 700;
  line-height: 120%;
  letter-spacing: 1%;
  text-transform: uppercase;
}

.main__content-text {
  margin: 0 0 40px;
  font-size: 28px;
  font-weight: 500;
  line-height: 120%;
  letter-spacing: 1%;
}

.main__picture {
  position: relative;
}

.main__picture-text {
  position: absolute;
  max-width: 155px;
  font-size: 16px;
  font-weight: 400;
  line-height: 140%;
  text-align: center;
}

.main__picture-text--first {
  top: 67px;
  left: 23px;
}

.main__picture-text--second {
  top: 50%;
  transform: translate(0, -50%);
  right: 10px;
}

.main__picture-text--third {
  left: 50%;
  transform: translate(-50%, 0);
  bottom: 67px;
}
</style>
