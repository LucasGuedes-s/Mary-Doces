<template>
  <div>
    <NavBar />

    <div class="home-inicio">
    </div>
  </div>

</template>

<script>
import NavBar from '@/components/NavBar.vue';
export default {
  name: 'HomeView',
  components: {
    NavBar
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
.home-inicio img {
  width: 70%;
}
</style>
