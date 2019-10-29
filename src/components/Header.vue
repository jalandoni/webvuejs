<template>
  <nav>
       <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    
  </nav>
</template>

<style>
nav{
    background-color:  #9999ff;
    height: 60px;
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

*{
      box-sizing:border-box;
      margin:0;
  }
</style>