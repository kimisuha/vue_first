<template>
  <div class="home mt-4 m-auto">
    <div class="card mb-3">
      <h1 class="card-title"> {{ this.text.title }} </h1>
      <p class="card-text">{{ this.text.content }}</p>
    </div>
  </div>
  <Navbar />
</template>

<script>
import Navbar from "../components/navbar.vue";
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
//import  from "../components/header.vue";

export default {
  name: "Home",
  components: {
    Navbar,
  },
  data() {
    return {
      text: { }
    }
  },
  mounted() {
    return this.text = JSON.parse(localStorage.getItem("text"));
  }
};
</script>
<style lang="css">
.home {
  text-transform: capitalize;
  font-family: "Times New Roman";
  width: 22rem;
  text-align: start;
  margin: auto 1rem;
}
.home h1, p {
  margin-left: 0.5rem;
}
</style>
