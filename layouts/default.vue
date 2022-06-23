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
  } else if (e.key === "d" && e.metaKey) {
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
  head() {
    return {
      title: "Ben Chomsang",
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,500;0,900;1,100;1,400;1,900&family=Public+Sans:ital,wght@0,100;0,500;0,900;1,100;1,400;1,900&display=swap");

html {
  font-family: "Poppins", sans-serif;
  font-weight: 200;
}

h1,
h2 {
  font-weight: 900;
}

.button {
  @apply px-6 py-3 bg-black text-white rounded-full;
}

.container {
  @apply p-16 rounded-xl mx-auto max-w-6xl;
}

.form {
  @apply px-6 py-3 bg-white rounded-lg border focus:border-black focus:outline-none;
}
</style>
