<template lang="en">
    <div class="header">
        <h1><router-link to="{ name: Home }">home</router-link></h1>
        <div class="item">
            <ul>
            <li><router-link :to="{ name: 'About' }">about</router-link></li>
            <li><a>private</a></li>
        </ul>
        </div>
    </div>
</template>
<script>
export default {
  name: "header",
};
</script>
<style>
.header {
  background: black;
  color: white;
  font-family: "Arial Narrow";
  text-transform: capitalize;
  display: flex;
  align-items: center;
}
.header a {
  text-decoration: none;
  cursor: pointer;
  text-align: start;
  margin-left: 0.5rem;
}
.header h1 {
  font-size: x-large;
}
.header .item {
  margin-left: auto;
}
.header .item ul {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
}
.header .item ul li {
  font-size: large;
  margin-right: 1rem;
  list-style: none;
}
</style>>