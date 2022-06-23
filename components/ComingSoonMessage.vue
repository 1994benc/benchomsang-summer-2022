<template>
  <div class="bg-yellow-50 p-10 text-yellow-500 rounded">
    <span class="font-black mr-4">Coming soon</span> {{ message }}
  </div>
</template>

<script>
export default {
  name: "ComingSoonMessage",
  props: {
    message: String,
  },
};
</script>
