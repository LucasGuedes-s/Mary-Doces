<template>
    <div class="container">
      <div class="nav">
        <img src="@/assets/logo.png" alt="Nav Image" href="/">
        <div class="text-nav">
          <router-link to="/pedido"><a>Realizar Pedido</a></router-link>
          <router-link to="/"><a>Contatos</a></router-link>
          <router-link to="/"><a>Sobre nós</a></router-link>
        </div>
      </div>
    </div>
</template>
<script>
export default {
  name: 'HomeView',
  components: {
  }
}
</script>
<style>
  .nav {
    position: absolute;
    width: 100%;
    margin: 0;
    margin-bottom: 200px; /* ajuste o valor conforme necessário */
    display: flex;
    align-items: center;
  }
  .nav img {
    float: left;
    height: 150px;
    margin-left: 50px;
  }
  .nav a {
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 19px;
    text-decoration: none;
    color: #9666ca;
    margin-right: 20px;
  }
  .text-nav{
    margin-left: 50px;
  }
  @media (max-width: 767px) {
    .nav a{
      display: none;
    }
    .nav img{
      margin: auto;
    }
  }
</style>
  