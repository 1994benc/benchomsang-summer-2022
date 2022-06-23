<template>
  <Intro />
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
});
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,500;0,900;1,100;1,400;1,900&family=Public+Sans:ital,wght@0,100;0,500;0,900;1,100;1,400;1,900&display=swap");

html {
  font-family: "Poppins", sans-serif;
  font-weight: 200;
}

h1, h2 {
  font-weight: 900;
}

.button {
  @apply px-6 py-3 bg-black text-white rounded-full;
}

.container {
  @apply p-16 rounded-xl mx-auto border max-w-5xl;
}
</style>
