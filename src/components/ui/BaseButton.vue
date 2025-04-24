<script setup>
import Button from "primevue/button";

const props = defineProps({
  label: String,
});
</script>
<template>
  <Button :label="props.label" class="base__btn" />
</template>
<style lang="scss" scoped>
.base__btn {
  min-width: 260px;
  padding: 15px 32px;
  font-size: 20px;
  font-weight: 700;
  line-height: 120%;
  background-color: var(--success);
  border-color: var(--success);
  border-radius: 8px;
  color: var(--text-light);
}
</style>
