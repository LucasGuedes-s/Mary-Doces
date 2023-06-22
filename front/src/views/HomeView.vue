<template>
  <div>
    <NavBar />
    <div class="home-inicio">
      <h1>A felicidade bate à sua porta. Faça seu pedido online e aproveite!</h1>
      <img src="@/assets/home.png">
      <h2>Confeitaria Mary Doces: adoçando sua vida, entregando felicidade!</h2>
    </div>
  </div>

</template>

<script>
import NavBar from '@/components/NavBar.vue';
export default {
  name: 'HomeView',
  components: {
    NavBar,
  }
}
</script>
  <style>
  .home-inicio {
    position: absolute;
    top: 100px;
    left: 0;
    right: 0;
    bottom: 0;
  }
  .home-inicio h1 {
    width: 40%;
    color: #9666ca;
    margin-top: 150px;
    margin-left: 50px;
    float: left;
  }
  .home-inicio h2 {
    width: 40%;
    font-size: 15px;
    color: #9666ca;
    margin-top: 150px;
    margin-left: 50px;
  }
  .home-inicio img {
    width: 35%;
    margin-right: 100px;
    float: right;
  }
  @media (max-width: 767px) {
    .home-inicio img {
      width: 75%;
      margin: 20px auto;
      float: none;
    }
    .home-inicio h1 {
      font-size: 15px;
      width: auto;
      margin: 40px auto;
    }
    .home-inicio h2{
      display: none;
    }
  }
</style>
