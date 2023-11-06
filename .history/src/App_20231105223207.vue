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
.flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100vw;
}
header {
  font-size: 1.7rem;
  justify-self: flex-end;
  width: 20%;
}

nav {
  padding: 30px;
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
body {
  font-family: sans-serif;
  height: 100vh;
  background: #261c33;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  text-align: center;
}
nav a {
  font-weight: bold;
  color: #fff;
  text-decoration: none;
  border-radius: 8px;
  background-color: #56447092;
  padding: 10px 20px;
  align-self: flex-end;
}
a:hover {
  color: rgba(137, 147, 200, 0.7);
}

nav a.router-link-exact-active {
  color: #8d81f3;
}
</style>
