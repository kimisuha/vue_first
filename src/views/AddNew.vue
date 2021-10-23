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
        />
      </div>

      <div class="form-group mb-3">
        <label for="content" class="form-label">content</label>
        <textarea
          name="content"
          rows="10"
          class="form-control"
          placeholder="input content here!"
        ></textarea>
      </div>
      <button type="button" class="btn btn-primary mx-auto d-block mb-3">
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
/* .addnew button{
    margin-left: 25rem;
} */
</style>