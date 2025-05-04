<template>
  <div>
    <Navbar :logo="logo_src" :alt="app_name" />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Navbar,
    Footer
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burger"
    }
  }
}
</script>

<style>
* {
  font-family: Helvetica;
  padding: 0;
  /* Zeramos todo padding */
  margin: 0;
  /* Zeramos toda margem */
  box-sizing: border-box;
  /* Serve para os inputs n passarem da largura máxima da div pai */
}

.main-container {
  margin: 50px;
  min-height: 300px;
  /* Com isso jogamos o footer para baixo, caso n estiver assim verifique se Home está acima do Footer em tags no componente App */
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}

body {
  scrollbar-width: thin;
  scrollbar-color: #FCBA03 #222;
}

/* Estilo da barra de rolagem inteira */
::-webkit-scrollbar {
  width: 10px;
  background-color: #222;
  /* fundo da barra */
}

/* Estilo da parte "deslizável" da barra */
::-webkit-scrollbar-thumb {
  background-color: #FCBA03;
  /* cor do polegar */
  border-radius: 6px;
}

/* Quando passar o mouse */
::-webkit-scrollbar-thumb:hover {
  background-color: #ff8800;
}
</style>