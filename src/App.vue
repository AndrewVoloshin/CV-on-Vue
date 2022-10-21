<template>
  <div id="app">
    <div id="nav">
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Lato, "Helvetica Neue", Helvetica, Arial, sans-serif;
  color: #939393;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.75;
}

* {
  box-sizing: border-box;
  padding: 0px;
  margin: 0px;
  border: none;
}

li {
  list-style-type: none;
}

a {
  color: red;
  color: #939393;
  text-decoration: none;
}

h1 {
  font-size: 44px;
  line-height: 0.91;
}

// #nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>
