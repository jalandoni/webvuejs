<template>
  <nav>
      <div id="nav">
      <router-link to="/">Head</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    
  </nav>
</template>

<style>


#nav {
  padding: 100px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

/* *{
      box-sizing:border-box;
      margin:0;
  } */
</style>