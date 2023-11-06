<template>
  <header>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
  </header>
  <router-view />
</template>

<style>
#app {
  text-align: center;
  z-index: 1;
  color: white;
}

nav {
  padding: 30px;
  position: fixed;
  top: 0;
  left: 50%;
}

nav a {
  font-weight: bold;
  color: #fff;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
