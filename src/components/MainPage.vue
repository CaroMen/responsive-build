<template>
  <div>
    <section id="welcome" class="grid">
      <div class="welcome-text">
        <h2>Developer</h2>
        <p
          class="l"
        >Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid beatae nostrum necessitatibus repudiandae facilis tempore.</p>
        <a href="#" class="button">View my work</a>
      </div>
    </section>
    <section id="portfolio">
      <h3>Some of my Projects</h3>
      <div class="projects grid">
        <a href>
          <img :src="require('@/assets/shaka.png')" alt />
          <h4>Sorting Visualizer</h4>
        </a>
        <a href>
          <img :src="require('@/assets/temp-photo.jpeg')" alt />
          <h4>Moxi Web</h4>
        </a>
        <a href>
          <img :src="require('@/assets/temp-photo-2.jpeg')" alt />
          <h4>Insta Clone</h4>
        </a>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data: () => ({
    // photo1: require("@/assets/shaka.png"),
  }),
};
</script>