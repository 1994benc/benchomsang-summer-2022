<template>
  <span class="text-gray-800 bg-gray-400 rounded px-1">{{ label }}</span>
</template>

<script>
export default {
  name: "KeyboardShortcutBadge",
  props: {
    label: String
  }
};
</script>
