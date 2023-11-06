<template>
  <css-doodle>
    :doodle { @grid: 1x3 / 100vmax; position: absolute; top: 0; left: 0;
    z-index: 0; } @size: 100% 150%; position: absolute; background: @m(100, (
    linear-gradient(transparent, @p( #FFFDE1@repeat(2, @p([0-9a-f])),
    #FB3569@repeat(2, @p([0-9a-f])) )) @r(0%, 100%) @r(0%, 100%) / @r(1px)
    @r(23vmin) no-repeat )); will-change: transform; animation: f 50s linear
    calc(-50s / @size() * @i()) infinite; @keyframes f { from { transform:
    translateY(-100%) } to { transform: translateY(100%) } }
  </css-doodle>

  <script src="https://unpkg.com/css-doodle@0.6.1/css-doodle.min.js"></script>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
