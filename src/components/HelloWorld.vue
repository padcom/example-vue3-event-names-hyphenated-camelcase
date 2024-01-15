<template>
  <h1>Hello, world! {{ message }}</h1>
  <button @click="$emit('helloWorld')">Say hello</button>
</template>

<script lang="ts" setup>
defineProps({
  message: { type: String, default: 'from HelloWorld.vue' },
})

defineEmits(['helloWorld'])
</script>

<style lang="postcss" scoped>
h1 {
  font-size: 1.875rem;
  line-height: 2.25rem;
}
</style>
