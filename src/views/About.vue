<template>
  <div class="about card m-auto mb-3 mt-4">
    <h1>first project todolist use vuejs</h1>
    <p>date create: 23/10/2021</p>
    <p>author: bui thanh loc B1906514</p>
    <p>time 2h20'</p>
  </div>
  <Navbar />
</template>
<script>
import Navbar from '../components/navbar.vue';
export default {
  name: 'About',
  components: { Navbar }
};
</script>
<style>
.about {
  text-transform: capitalize;
  width: 22rem;
  text-align: center;
}
</style>
