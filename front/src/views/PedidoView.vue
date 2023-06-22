<template>
  <div class="about">
    <NavBar />
  </div>
  <div>
    <PedidosVue />
  </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue';
import PedidosVue from '@/components/Pedido.vue';
  export default {
    data(){
    },
    components: {
      NavBar,
      PedidosVue
    }
  }
</script>
<style>
</style>