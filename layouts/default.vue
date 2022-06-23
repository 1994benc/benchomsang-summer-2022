<template>
  <div>
    <nav class="py-6 px-10 mb-10">
      <NuxtLink to="/"><div class="left">Ben Chomsang</div></NuxtLink>
      <div class="right"></div>
    </nav>
    <Nuxt />
  </div>
</template>

<script>
const handleUserKeyDown = function (e) {
  e.preventDefault();
  if (e.key === "a" && e.metaKey) {
    this.$router.push("/software");
  } else if (e.key === "b" && e.metaKey) {
    this.$router.push("/plants");
  } else if (e.key === "c" && e.metaKey) {
    this.$router.push("/journey");
  } else if (e.key === "h" && e.metaKey) {
    this.$router.push("/");
  } else if (e.key === 'd' && e.metaKey) {
    this.$router.push("/contact");
  }
};

export default {
  name: "default",
  mounted() {
    console.log("Default layout created");
    window.addEventListener("keydown", handleUserKeyDown.bind(this));
  },
  beforeDestroy() {
    console.log("Default layout destroyed");
    window.removeEventListener("keydown", handleUserKeyDown.bind(this));
  },
};
</script>
