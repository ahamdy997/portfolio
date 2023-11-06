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
/* #app {
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  text-align: center;
} */
.flex {
  display: flex;
  align-items: center;
  justify-content: space-around;
  padding: 3rem;
  gap: 5rem;
  width: 100%;
  margin-left: 3rem;
}
header {
  font-size: 1.7rem;
}

nav {
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 20%;
}
body {
  font-family: sans-serif;
  background: #261c33;
  color: #fff;
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
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
  color: rgba(137, 147, 200, 0.7);
}

nav a.router-link-exact-active {
  color: #8d81f3;
}
</style>
