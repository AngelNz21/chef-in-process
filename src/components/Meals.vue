<template>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-5 px-8">
    <MealItem v-for="meal of meals" :key="meal.idMeal" :meal="meal" />
  </div>
  <div v-if="!meals.length" class="flex justify-center text-gray-800 p-8">
    There are no recipes
  </div>
</template>

<script setup>
import MealItem from "./MealItem.vue";

const { meals } = defineProps({
  meals: {
    required: true,
    type: Array,
  },
});
</script>
