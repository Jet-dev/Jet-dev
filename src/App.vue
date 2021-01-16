<template>
<!--  <div id="nav">-->
<!--    <router-link to="/">Home</router-link> |-->
<!--    <router-link to="/about">About</router-link>-->
<!--  </div>-->
  <router-view />
</template>

<style>
#app {
  font-family: "Press Start 2P", serif;
  text-align: center;
  color: white;
}

@font-face {
  font-family: "Press Start 2P";
  src: url("assets/PressStart2P-Regular.ttf");
}

html {
  cursor: url("../node_modules/nes.css/assets/cursor.png"),auto;
}

body {
  background-color: #212529;
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
