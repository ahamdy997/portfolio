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
  color: white;
}
header {
  font-size: 25px;
  width: 100%;
}
nav {
  padding: 30px;
  text-align: center;
}
body {
  font-family: sans-serif;
  height: 100vh;
  margin: 0;
  background: #261c33;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
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
  color: rgba(137, 147, 200, 0.7);
}

nav a.router-link-exact-active {
  color: #8d81f3;
}
</style>
