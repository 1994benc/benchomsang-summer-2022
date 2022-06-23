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
  if (e.key === "a") {
    this.$router.push("/software");
  } else if (e.key === "b") {
    this.$router.push("/plants");
  } else if (e.key === "c") {
    this.$router.push("/journey");
  } else if (e.key === "h") {
    this.$router.push("/");
  }
};

export default {
  name: "default",
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
