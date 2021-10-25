<template>
  <div class="addnew mt-4">
    <form action="#">
      <div class="form-group mb-3">
        <label for="title" class="form-label">title</label>
        <input
          type="text"
          class="form-control"
          name="title"
          placeholder="input a title!"
          v-model="title"
        />
      </div>

      <div class="form-group mb-3">
        <label for="content" class="form-label">content</label>
        <textarea
          name="content"
          rows="10"
          class="form-control"
          placeholder="input content here!"
          v-model="content"
        ></textarea>
      </div>
      <button type="button" class="btn btn-primary mx-auto d-block mb-3" v-on:click="add">
        add
      </button>
    </form>
    <Navbar />
  </div>
</template>
<script>
import Navbar from "../components/navbar.vue";
export default {
  components: { Navbar },
  name: "AddNew",
  data() {
    return {
      text: { }
    }
  },
  methods: {
    add(){
      this.text.title = this.title;
      this.text.content = this.content;
      localStorage.setItem("text", JSON.stringify(this.text));
      console.log(JSON.parse(localStorage.getItem("text")));
      window.location.href = 'http://192.168.88.102:8080/';
    },
  },
};
</script>
<style lang="css">
.addnew {
  margin: auto 1rem;
  text-transform: capitalize;
  font-family: "Times New Roman";
}
.addnew label {
  font-size: larger;
  margin-left: 0.5rem;
}
</style>