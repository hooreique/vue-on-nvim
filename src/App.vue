<script setup lang="ts">
import { ref } from 'vue'

const cnt = ref<number>(0)
</script>

<template>
  <p>node + typescript + neovim + lsp</p>

  <button @click="cnt++">{{ cnt }}</button>
</template>
