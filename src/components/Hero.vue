<template>
  <div class="hero">
    <section class="jumbo">
      <h1 class="jumbo-title">{{ heroTitle }}</h1>
      <p class="jumbo-text">{{ heroText }}</p>
    </section>
  </div>
</template>

<script>
export default {
  name: "AppHero",
  props: {
    heroTitle: String,
    heroText: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section.jumbo {
  color: white;
  height: 70vh;
  position: relative;
  background: url(http://localhost:8080/img/jumbo.f1c4cde2.jpg) center / cover;
}
section.jumbo h1.jumbo-title {
  top: 1rem;
  font-size: 2.5rem;
}

section.jumbo h1.jumbo-title,
section.jumbo p.jumbo-text {
  position: absolute;
  left: 0.7rem;
}
section.jumbo p.jumbo-text {
  bottom: 1rem;
  font-size: 1.5rem;
}
</style>
