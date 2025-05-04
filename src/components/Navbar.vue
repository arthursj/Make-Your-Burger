<template>
    <div id="nav">
      <router-link to="/" id="logo-url">
        <img :src="logo" :alt="alt" id="logo">
      </router-link>
      <router-link to="/">Home</router-link> |
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </template>
  <script>
  export default {
    name: "Navbar",
    props: ["logo", "alt"]
  }
  </script>
  <style scoped>
    #nav {
      background-color: #222;
      border-bottom: 4px solid #111;
      padding: 15px 50px;
      display: flex;
      justify-content: flex-end;
      align-items: center;
    }
  
    #nav  #logo-url { /* Só com isso já temos ele jogado para left */
      margin: auto;
      margin-left: 0;
    }
  
    #logo {
      width: 40px;
      height: 40px;
    }

    #logo::selection,
    #nav a::selection,
    router-link {
      background-color: #FCBA03;
      color: #222;
    }
  
    #nav a {
      color: #FCBA03;
      text-decoration: none;
      margin: 12px;
    }
  
    #nav a:hover {
      color: #FFF;
    }
  </style>
  