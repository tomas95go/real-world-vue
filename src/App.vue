<template>
  <section class="section">
    <div class="container">
      <div class="columns is-centered">
        <router-link class="button is-outlined is-link mr-1" to="/"> Event List </router-link>
        <router-link class="button is-outlined is-link ml-1" to="/about"> About </router-link>
      </div>
      <div class="columns is-centered">
        <router-view />
      </div>
    </div>
  </section>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
