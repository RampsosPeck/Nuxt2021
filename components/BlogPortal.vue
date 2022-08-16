<template>
  <div class="portalBlog">
    <p>Nro.{{id}}</p>
    <nuxt-link :to="'/blog/'+id"> <h1>{{title}}</h1></nuxt-link>
    <p> {{body}}</p>
    <nuxt-link :to="'/blog/'+id" class="readmore_item"><p class="read"> Leer mas...</p></nuxt-link>
  </div>
</template>

<script>
export default {

  props: ["title","body", "id"]

}
</script>

<style scoped>
.portalBlog{
  border: 1px solid black;
  padding: 10px;
}

.readmore_item{
  text-decoration: none;
  list-style-type: none;
}

.read{
  font-size: 20px;
  background-color: crimson;
  border-radius: 20px;
  padding: 10px;
  width: 120px;
  color: white;
  align-items: center;
  text-align: center;
}

.read:hover{
  font-size: 20px;
  background-color: rgb(190,220,20);
  border-radius: 20px;
  padding: 10px;
  width: 120px;
  color: white;
  align-items: center;
  text-align: center;
}

</style>





