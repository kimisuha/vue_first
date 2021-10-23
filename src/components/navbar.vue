<template>
  <div class="navb">
    <ul>
      <li><router-link to="/">home</router-link></li>
      <li><router-link to="add-new">addnew</router-link></li>
      <li><router-link to="About">About</router-link></li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "navbar",
};
</script>
<style lang="css">
.navb {
  text-transform: capitalize;
  font-family: "Times New Roman";
  margin: auto 1rem;
}
.navb ul {
  display: flex;
  justify-content: space-around;
  border: 1px solid black;
  background: black;
  border-radius: 0.5rem;
}
.navb li {
  list-style: none;
  font-size: larger;
  color: white;
}
.navb a {
  text-decoration: none;
  color: white;
}

.navb a:hover{
    text-decoration: underline;
}
</style>