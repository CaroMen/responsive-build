<template>
  <div class="navbar">
    <nav class="nav-extended z-depth-0">
      <div class="nav-content">
        <router-link to>
          <span class="nav-title text">Caro.</span>
        </router-link>
        <router-link to>
          <ul id="nav-mobile" class="right hide-on-med-and-down">
            <li>
              <router-link :to="{ name: '#' }">
                <a>Home</a>
              </router-link>
            </li>
            <li>
              <router-link :to="{ name: '#' }">
                <a>Portfolio</a>
              </router-link>
            </li>
            <li>
              <router-link active-class="active" :to="{ name: '#' }">
                <a>Contact</a>
              </router-link>
            </li>
          </ul>
        </router-link>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {};
  },
};
</script>

<style>
body {
  background-color: #f4f4f5;
  color: #c6a277;
}

.text {
  color: #c6a277;
}

.navbar nav {
  padding: 0 60px;
  font-family: Lato, Helvetica, Arial, sans-serif;
  background-color: #f4f4f5;
}

.nav-title {
  color: #48564f;
  font-size: 50px;
}

#nav-mobile {
  padding: 30px 10px;
  color: #c6a277;
}

/* iPad */
@media (min-device-width: 768px) and (max-device-width: 1024px) {
  .navbar nav {
    padding: 0 60px;
    font-family: Lato, Helvetica, Arial, sans-serif;
  }
  #nav-mobile {
    margin-top: -255px;
    padding: 90px 70px;
    margin-left: -100px;
  }
}

/* iPad Pro */
@media (min-device-width: 1024px) and (max-device-width: 1366px) and (-webkit-min-device-pixel-ratio: 2) {
  .navbar nav {
    padding: 0 60px;
    font-family: Lato, Helvetica, Arial, sans-serif;
  }
  #nav-mobile {
    margin-top: -55px;
    padding: 90px 70px;
  }
}
</style>
