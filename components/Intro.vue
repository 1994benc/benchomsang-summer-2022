<template>
  <div class="p-16 rounded-xl mx-auto border max-w-5xl">
    <h1 class="text-7xl">Hello friend 😊 What do you want to know about me?</h1>
    <div class="my-8">
      <button class="button">Software engineering <KeyboardShortcutBadge label="Press A" /></button>
      <button class="button">My house plants 🪴 <KeyboardShortcutBadge label="Press B" /></button>
      <button class="button">My journey <KeyboardShortcutBadge label="Press C" /></button>
    </div>
  </div>
</template>

<script>
import KeyboardShortcutBadge from './KeyboardShortcutBadge.vue';
export default {
    name: "Intro",
    components: { KeyboardShortcutBadge }
};
</script>
