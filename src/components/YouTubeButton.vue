<template>
  <a
    :href="href"
    target="_blank"
    class="px-3 py-2 border-2 text-white border-red-700 bg-red-600 hover:bg-red-700 transition-colors"
    id="ytbtn"
  >
    <slot>See Tutorial</slot>
  </a>
</template>

<script setup>
const props = defineProps({
  href: String,
});
</script>

<style>
#ytbtn {
  border-radius: 10px;
}
</style>