<template>
  
  <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
    <compheader/>
    <compslider/>
    <newscard/>
    <tourcard/>
    <hotelcard/>
    <compfooter/>

  <router-view />
</template>




<script>
  import compheader from '../components/compheader.vue';
  import compslider from '../components/compslider.vue';
  import compfooter from '../components/compfooter.vue';
  import tourcard from '../components/tourcard.vue';
  import newscard from '../components/newscard.vue';
  import hotelcard from '../components/hotelcard.vue';

export default {
  components: {
    compheader,
    compslider,
    tourcard,
    compfooter,
    newscard,
    hotelcard,
  }

}

</script>




<style>
</style>
