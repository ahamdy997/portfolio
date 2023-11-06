<template>
  <div class="flex">
    <router-view />
    <header>
      <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
      </nav>
    </header>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
#app {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  text-align: center;
}
.flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 3rem;
  gap: 5rem;
  width: 100%;
}
header {
  font-size: 1.7rem;
}

nav {
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  margin-right: 1.5rem;
}
body {
  font-family: sans-serif;
  background: #261c33;
  /* background: yellow; */
  color: #fff;
}
nav a {
  font-family: serif;
  font-weight: bold;
  color: #fff;
  text-decoration: none;
  font-size: 3rem;
  transition: font-style 0.2s;
}
a:hover {
  font-style: italic;
  transform: translateX(10px);
}

nav a.router-link-exact-active {
  color: #8d81f3;
}
</style>
