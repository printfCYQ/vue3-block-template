<script setup lang="ts">
defineProps<{ msg: string }>()

const fontSize = ref('30px')
</script>

<template>
  <h1>{{ msg }}</h1>
</template>
<style lang="scss" scoped>
$color :red;

h1 {
  color: $color;
  font-size: v-bind(fontSize);
}
</style>