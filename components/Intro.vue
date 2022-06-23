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

export default {
  name: "Intro",
  components: { KeyboardShortcutBadge },
};
</script>
