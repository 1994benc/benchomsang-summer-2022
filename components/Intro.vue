<template>
  <div class="container">
    <h1 class="text-7xl">Hello friend 😊 What do you want to know about me?</h1>
    <div class="my-8">
      <NuxtLink to="/software"
        ><button class="button">
          Software engineering <KeyboardShortcutBadge label="Press A" /></button
      ></NuxtLink>
      <NuxtLink to="/plants"
        ><button class="button">
          My house plants 🪴 <KeyboardShortcutBadge label="Press B" /></button
      ></NuxtLink>
      <NuxtLink to="/journey"
        ><button class="button">
          My journey <KeyboardShortcutBadge label="Press C" /></button
      ></NuxtLink>
    </div>
  </div>
</template>

<script>
import KeyboardShortcutBadge from "./KeyboardShortcutBadge.vue";

const handleUserKeyDown = function(e) {
  if (e.key === "a") {
    this.$router.push("/software");
  } else if (e.key === "b") {
    this.$router.push("/plants");
  } else if (e.key === "c") {
    this.$router.push("/journey");
  }
};
export default {
  name: "Intro",
  components: { KeyboardShortcutBadge },
  mounted() {
    console.log("Intro created");
    window.addEventListener("keydown", handleUserKeyDown.bind(this));
  },
  beforeDestroy() {
    console.log("Intro destroyed");
    window.removeEventListener("keydown", handleUserKeyDown.bind(this));
  },
};
</script>
