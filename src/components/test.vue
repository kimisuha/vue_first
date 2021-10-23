<template>
  <form action="#">
    <div class="mb-3">
        <label for="name" class="form-label">name</label>
        <input type="text" class="form-control" name="name">
    </div>
    <div class="mb-3">
        <label for="sdt" class="form-label" >sdt</label>
        <input type="tel" name="sdt"  class="form-control"/>
    </div>
    <div class="mb-3">
        <label for="email" class="form-label">email</label>
        <input type="email" name="email"  class="form-control"/>
    </div>
    <div class="mb-3">
        <label for="address" class="form-label">addres</label>
        <input type="text" name="address"  class="form-control"/>
    </div>
    <button type="button" class="btn btn-success">accesss</button>
  </form>
</template>
<script>

export default {
    name: "Test",
};
</script>
<style lang="scss">
</style>