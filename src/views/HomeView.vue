<script setup lang="ts">
import { ref } from 'vue'
// import ConnectComponent from "@/components/ConnectComponent.vue";

const show = ref(false)
const onError = (error: Error) => {
  console.debug({ error })
}
</script>
<template>
  <ConnectComponent @error="onError" :chain="5553" :model-value="true" />
</template>
