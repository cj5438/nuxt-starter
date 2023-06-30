<template>
  <nuxt-link to="/about">about</nuxt-link>
  <div>Hello Nuxt from page, auto generate routes: {{ store.count }}</div>
  <button class="btn px-4" @click="store.increment">+1</button>
</template>

<script lang="ts" setup>
// import { defineComponent } from 'vue'
import { useCounter } from '~/stores/useCounter'

const store = useCounter()

// export default defineComponent({
//   setup() {

//     return {}
//   }
// })
</script>

<style scoped lang="scss">
$width: 120px;
.btn {
  width: $width;
}
</style>
