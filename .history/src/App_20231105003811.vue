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
header {
  font-size: 25px;
  position: fixed;
  top: 10%;
  left: 0%;
  width: 100%;
}
nav {
  padding: 30px;
  text-align: center;
}

nav a {
  font-weight: bold;
  color: #fff;
  text-decoration: none;
  border-radius: 8px;
  background-color: #56447092;
  padding: 10px 20px;
}
a:hover {
  color: rgba(197, 147, 200, 0.8);
}

nav a.router-link-exact-active {
  color: #8d81f3;
}
</style>
