<template>
  <div id="app">
    
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/challenge-1">Challenge 1</router-link> | 
      <router-link to="/challenge-2">Challenge 2</router-link> | 
      <router-link to="/challenge-3">Challenge 3</router-link> |
      <router-link to="/final">Final</router-link>
    </div>
    <router-view/>
    <img id="insect" :src="require('./assets/insect.png')"/>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
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
#insect{
  position: absolute;
  height:300px;
  right: 0px;
  bottom: 0px;
}
</style>
