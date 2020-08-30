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
          <img :src="require('@/assets/urban.png')" alt />
          <h4>Sorting Visualizer</h4>
        </a>
        <a href>
          <img :src="require('@/assets/shaka.png')" alt />
          <h4>Moxi Web</h4>
        </a>
        <a href>
          <img :src="require('@/assets/podcast.png')" alt />
          <h4>Insta Clone</h4>
        </a>
      </div>
    </section>
    <section id="skills">
      <h3>Things I Can Do</h3>
      <ul class="grid">
        <li>JavaScript</li>
        <li>Python</li>
        <li>Dart</li>
        <li>Flutter</li>
        <li>Vue</li>
        <li>Django</li>
        <li>Firebase</li>
      </ul>
    </section>
    <section id="contact">
      <h3>Get in Touch</h3>
      <p class="leading">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Unde, velit!</p>
      <form>
        <input type="text" placeholder="NAME" />
        <input type="email" placeholder="EMAIL" />
        <textarea placeholder="YOUR MESSAGE"></textarea>
        <button class="button">Send Message</button>
      </form>
    </section>
    <footer>
      <div class="grid">
        <p class="copyright">Copyright 2020 Caro.</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data: () => ({
    // photo1: require("@/assets/shaka.png"),
  }),
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Rajdhani&display=swap");

/* variables  */
:root {
  --primary: #f4f4f5;
  --secondary: #c6a277;
}

/* images */
.shaka {
  width: 100%;
  height: 78%;
}

img {
  padding: 20px;
  width: 90%;
}

/* reset */
body,
p,
a,
ul,
li {
  margin: 0;
  padding: 0;
  text-decoration: none;
}

li {
  list-style-type: none;
}

/* base styles */
body {
  background: var(--primary);
  /* overflow-x: hidden; */
  font-family: "Rajdhani";
}

.button {
  background: none;
  border: 2px solid var(--secondary);
  color: var(--secondary);
  padding: 6px 12px;
  border-radius: 20px;
  text-transform: uppercase;
  box-shadow: 1px 2px 3px rgba(0, 0, 0, 0.2);
  display: inline-block;
}

.button:hover {
  color: #222;
  background: var(--secondary);
}

input,
textarea {
  background: rgba(255, 255, 255, 0.05);
  padding: 10px 16px;
  border-radius: 20px;
  border: 2px solid #48564f;
}

/* fonts */
@font-face {
  font-family: "Raj Medium";
  src: url("/assets/fonts/Rajdhani-Medium.ttf");
}

h1,
h2,
h3,
h4 {
  color: #151515;
  font-weight: normal;
}

p,
a,
li {
  color: #302e2e;
}

h1,
h3 {
  font-size: 1.2em;
}

h2 {
  font-size: 1.6em;
}
h4 {
  font-size: 1.1em;
}

.leading {
  font-size: 1.1em;
}

/* mobile styles */

/* small tablet styles */
@media screen and (min-width: 620px) {
}

/* large tablets and laptops*/
@media screen and (min-width: 960px) {
  body {
    font-size: 18px;
  }
}

/* desktop styles */

@media screen and (min-width: 1200px) {
  body {
    font-size: 20px;
  }
}

/* grid testing */
.projects {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 10px;
}

.projects a {
  text-align: center;
  padding: 20px;
}
</style>