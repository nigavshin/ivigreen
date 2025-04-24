<script setup>
import BaseButton from "./ui/BaseButton.vue";
import BaseCarousel from "./ui/BaseCarousel.vue";
import Topics from "./Topics.vue";
</script>

<template>
  <section class="why">
    <div class="why__container container">
      <h2 class="why__title subtitle">Why Ivi Green?</h2>
      <ul class="why__list">
        <li class="why__item">
          <strong class="why__item-accent">40 000+</strong>
          <p class="why__item-description">
            products sold all around the world
          </p>
        </li>
        <li class="why__item">
          <strong class="why__item-accent">1 000+</strong>
          <p class="why__item-description">teachers use Ivi Green products</p>
        </li>
        <li class="why__item">
          <strong class="why__item-accent">30+</strong>
          <p class="why__item-description">
            countries use our toolkits to effectively teach
          </p>
        </li>
      </ul>
      <ul class="why__cards">
        <li class="why__card">
          <strong class="why__card-accent"
            >The challenges teachers are facing</strong
          >
          <p class="why__card-description">
            Teachers often face the challenge of spending extensive time
            searching for quality materials for their classes while students
            frequently approach them with more and more questions about their
            emotions, conflicts, self-organization methods, and family or friend
            relationships. The pandemic has exacerbated social-emotional
            problems among kids, making SEL one of the priorities for the school
            curriculum. Now even teachers specializing in subjects like math
            or language art need to incorporate social-emotional basics into
            their instructions.
          </p>
        </li>
        <li class="why__card">
          <strong class="why__card-accent">Our solution</strong>
          <p class="why__card-description">
            Our toolkits provide teachers with practical, visual, science-based
            resources to effectively teach social and emotional learning
            to teens. Designed to enhance emotional intelligence and build
            resilience, Ivi Green educational toolkits offer structured
            activities, comprehensive guidelines, and ready-to-use materials
            that cater to the unique developmental needs of adolescents.
            Educators can foster a supportive learning environment that promotes
            emotional well-being and academic success by integrating these tools
            into their teaching.
          </p>
        </li>
      </ul>
      <BaseButton label="Show all kits" class="why__btn" />
      <BaseCarousel />
      <Topics />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.why {
  padding: 40px 0;
  background-color: var(--background-light);
}

.why__list {
  margin: 0 0 32px;
  display: flex;
  justify-content: space-between;
}

.why__item {
  max-width: 284px;
  text-align: center;
}

.why__item-accent {
  margin: 0 0 10px;
  font-size: 64px;
  font-weight: 700;
  color: var(--success);
}

.why__item-description {
  font-size: 20px;
  font-weight: 500;
  color: var(--text-dark);
}

.why__cards {
  margin: 0 0 40px;
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.why__card {
  padding: 40px;
  border-radius: 20px;
  background-color: var(--background-grey-2);
}

.why__card-accent {
  margin: 0 0 20px;
  font-size: 28px;
  font-weight: 500;
  line-height: 120%;
  letter-spacing: 1%;
  color: var(--general);
}

.why__card-description {
  font-size: 16px;
  font-weight: 400;
  line-height: 140%;
}

.why__btn {
  margin: 0 auto;
  display: block;
}
</style>
