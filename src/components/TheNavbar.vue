<template>
  <div id="nav">

  <a href="">
      <img src="@/assets/SVGlogo.svg" alt="">
    </a>

     <button class="nav-button">
         Get In Touch
     </button>  
  </div>
</template>

<script>
export default {
    name: 'navbar'

}
</script>

<style lang="scss" scopped>
#nav {
  display: flex;
  padding: 25px;
  justify-content: space-between;
}

  button {

    background: #022836;
    color: white;
    font-family: Montserrat;
    border: 2px solid #7ED9DA;
    font-size: 20px;
    padding: 10px 20px;
  }

  @media screen and (max-width: 900px) {
    .nav-button {
      display: none;
    }
    a {
      margin: auto;
    }
  }
</style>