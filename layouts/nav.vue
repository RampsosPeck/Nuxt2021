<template>
  <nav class="navbar">
    <ul class="navitems">
      <nuxt-link to="/" class="each-items"><li>Home</li></nuxt-link>
      <nuxt-link to="/about" class="each-items"><li>About</li></nuxt-link>
      <nuxt-link to="/contact" class="each-items"><li>Contact</li></nuxt-link>
      <nuxt-link to="/blog" class="each-items"><li>Blog</li></nuxt-link>
    </ul>
  </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
.navbar{
  height: 8vh;
  background-color: crimson;
  justify-content: space-around;
  display: flex;
}
.navitems{
  display: flex;
  justify-content: space-around;
  list-style-type: none;
  width: 30%;
  color:white;
  align-items: center;
}

.each-items{
  text-decoration: none;
  color: white;
}

.each-items:hover{
  /*color: rgb(255, 255, 255);*/
  border: 1px solid white;
  /*padding: 5px;*/
}

</style>





