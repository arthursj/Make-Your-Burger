<template>
 <div id="footer">
   <p>Make Your Burger &copy; 2025</p>
 </div>
</template>
<script>
  export default {
   name: "Footer"
  }
</script>

<style scoped>
  #footer {
    height: 201px;
    background-color: #222;
    border-top: 4px solid #111;
    color: #FCBA03;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
  }

  #footer::selection {
    background-color: #FCBA03;
    color: #222;
  }
</style>
