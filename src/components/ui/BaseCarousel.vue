<template>
  <div class="base-carousel">
    <Carousel
      :value="images"
      :numVisible="1"
      :numScroll="1"
      :circular="false"
      :showIndicators="false"
    >
      <template #item="slotProps">
        <img :src="slotProps.data.image" :alt="slotProps.data.id" />
      </template>
      <template #previcon>
        <svg width="80" height="80" viewBox="0 0 80 80" fill="none">
          <rect width="80" height="80" rx="40" fill="#32CD7A" />
          <path
            d="M32.2819 38.115C32.376 38.0183 32.7316 37.605 33.0628 37.265C35.0047 35.1267 40.0705 31.6267 42.7219 30.5583C43.1245 30.3867 44.1426 30.0233 44.6865 30C45.2077 30 45.7045 30.12 46.1786 30.3633C46.7696 30.7033 47.2437 31.2383 47.5035 31.87C47.6707 32.3083 47.9305 33.62 47.9305 33.6433C48.1903 35.0783 48.3332 37.41 48.3332 39.9867C48.3332 42.4417 48.1903 44.6783 47.9776 46.135C47.9532 46.1583 47.6935 47.7883 47.4093 48.3467C46.8881 49.3667 45.8701 50 44.7806 50H44.6865C43.9769 49.975 42.4848 49.3417 42.4848 49.3183C39.9763 48.2483 35.0274 44.92 33.0385 42.7083C33.0385 42.7083 32.4783 42.14 32.2348 41.785C31.8548 41.275 31.6665 40.6433 31.6665 40.0117C31.6665 39.3067 31.8792 38.65 32.2819 38.115Z"
            fill="white"
          />
        </svg>
      </template>
      <template #nexticon>
        <svg width="80" height="80" viewBox="0 0 80 80" fill="none">
          <rect
            width="80"
            height="80"
            rx="40"
            transform="matrix(-1 0 0 1 80 0)"
            fill="#32CD7A"
          />
          <path
            d="M47.7181 38.115C47.624 38.0183 47.2684 37.605 46.9372 37.265C44.9953 35.1267 39.9295 31.6267 37.2781 30.5583C36.8755 30.3867 35.8574 30.0233 35.3135 30C34.7923 30 34.2955 30.12 33.8214 30.3633C33.2304 30.7033 32.7563 31.2383 32.4965 31.87C32.3293 32.3083 32.0695 33.62 32.0695 33.6433C31.8097 35.0783 31.6668 37.41 31.6668 39.9867C31.6668 42.4417 31.8097 44.6783 32.0224 46.135C32.0468 46.1583 32.3065 47.7883 32.5907 48.3467C33.1119 49.3667 34.1299 50 35.2194 50H35.3135C36.0231 49.975 37.5152 49.3417 37.5152 49.3183C40.0237 48.2483 44.9726 44.92 46.9615 42.7083C46.9615 42.7083 47.5217 42.14 47.7652 41.785C48.1452 41.275 48.3335 40.6433 48.3335 40.0117C48.3335 39.3067 48.1208 38.65 47.7181 38.115Z"
            fill="white"
          />
        </svg>
      </template>
    </Carousel>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Carousel from "primevue/carousel";

const images = ref([
  {
    id: "0",
    image: "src/assets/slide-1.jpg",
  },
  {
    id: "1",
    image: "src/assets/slide-2.jpg",
  },
  {
    id: "2",
    image: "src/assets/slide-3.jpg",
  },
  {
    id: "3",
    image: "src/assets/slide-4.jpg",
  },
  {
    id: "4",
    image: "src/assets/slide-5.jpg",
  },
]);
</script>

<style lang="scss" scoped>
.base-carousel {
  margin: 100px 0;
}

::v-deep(.p-carousel) {
  .p-carousel-item {
    img {
      width: 100%;
      height: 550px;
      object-fit: cover;
      border-radius: 20px;
    }
  }

  .p-carousel-viewport {
    margin: 0 20px;
  }

  .p-carousel-prev-button,
  .p-carousel-next-button {
    width: 80px;
    height: 80px;
  }
}
</style>
