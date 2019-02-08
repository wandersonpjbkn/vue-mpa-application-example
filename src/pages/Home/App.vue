<template>
  <div id="app">
    <img
      alt="Vue logo"
      src="@/assets/logo.png"
    >

    <div style="position: relative">
      <div class="short-it">
        <HelloWorld msg="Welcome to Your Vue.js App" />
      </div>
      <div />
    </div>

    <nav>
      <ul>
        <li>Go to</li>
        <li>
          <a
            href="about.html"
          >
            About Us
          </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.short-it {
  position: relative;

  overflow-x: hidden;
  overflow-y: auto;
  max-height: 300px;

  + div {
    position: absolute;
    bottom: 0;
    z-index: 1;

    display: block;
    width: 100%;
    height: 40px;
    background-image: linear-gradient(to bottom, transparent, #fff)
  }

}

nav ul {
  margin-top: 30px
}
</style>
