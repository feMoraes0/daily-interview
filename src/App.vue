<template>
  <main class="container">
    <v-header></v-header>
  </main>
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core';
import vHeader from "@/components/Header.vue";

export default defineComponent({
  components: {
    vHeader
  }
});
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');

* {
  box-sizing: inherit;
  margin: 0;
  padding: 0;
}

html {
  font-size: 62.5%;
}

body {
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  width: 100vw;
  min-height: 100vh;
  overflow-x: hidden;

  &::before {
    background-color: #F78F8F;
    content: '';
    height: 30vh;
    position: absolute;
    width: 100vw;
    z-index: -1;
  }
}

.container {
  width: 80%;
  margin: 0 auto;
  padding-top: 15px;
}
</style>
