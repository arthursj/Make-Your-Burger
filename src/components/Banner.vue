<template>
  <div id="main-banner">
    <h1>Make Your Burger</h1>
  </div>
</template>

<script>
export default {
  name: "Banner"
}
</script>

<style scoped>

  #main-banner {
    background-image: url('../../public/img/burger.jpg');
    background-position: 0 -250px;
    background-size: cover;
    height: 610px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }

  #main-banner h1 {
    color: #FFF;
    text-align: center;
    font-size: 60px;
    background-color: #222;
    padding: 20px 40px;
  }

  #main-banner h1::selection {
    background-color: #fcba03;
    color: #222;
  }

  @media (max-width: 1350px) {
    #main-banner {
      background-position: -500px -500px;
      height: 200px;
    }
  }
  @media (max-width: 1329px) {
    #main-banner {
      background-position: -500px -250px;
      background-size: cover;
      background-repeat: no-repeat;
      height: 900px;
    }
    #main-banner h1 {
      padding: 10px 20px;
      margin-bottom: 400px;
    }
  }
  @media (max-width: 1328px) {
    #main-banner {
      background-position: 0px -250px;
    }
  }
  @media (max-width: 729px) { /* 729px */
    #main-banner {
      height: 1000px;
      background-position: -700px -250px;
    }
    #main-banner h1 {
      font-size: 50px;
    }
}
</style>
