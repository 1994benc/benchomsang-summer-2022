<template>
  <div class="container">
    <h1 class="text-7xl">Hi 👋 How do you want to know me?</h1>
    <div class="my-8 flex gap-3 flex-wrap items-center">
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
      <NuxtLink to="/contact"
        ><button class="button">
          Contact me <KeyboardShortcutBadge label="Press D" /></button
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
