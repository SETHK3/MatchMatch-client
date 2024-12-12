<template>
  <div class="home">
    <div class="navbar-wrapper">
      <div class="navbar-logo">
        <!-- <img src="" alt="logo" class="logo" /> -->
        <h1>MatchMatch</h1>
      </div>
      <div class="nav-links">
        <a href="#">Home</a>
        <a href="#">Tabs</a>
        <a href="#">Tabs</a>
        <a href="#">Tabs</a>
      </div>
      <button class="account">Create Account</button>
    </div>

    <div class="main-content">
      <div class="logo-toggle">
        <a href="https://vite.dev" target="_blank">
          <img src="/vite.svg" class="logo" alt="Vite logo" />
        </a>
        <a href="https://vuejs.org/" target="_blank">
          <img src="./../assets/vue.svg" class="logo vue" alt="Vue logo" />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.home {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: Lexend, sans-serif;
  color: #272d41;
  width: 100%;
  box-sizing: border-box;
}

.navbar-wrapper {
  position: fixed;
  width: 100%;
  z-index: 1;
  background-color: white;

  .navbar-logo {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    padding: 1rem 1rem;
    background-color: white;
    border-bottom: 1px solid gray;
    box-sizing: border-box;
  }
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
