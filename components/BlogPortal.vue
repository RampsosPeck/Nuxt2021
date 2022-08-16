<template>
  <div class="portalBlog">
    <p>Nro.{{id}}</p>
    <nuxt-link :to="'/blog/'+id"></nuxt-link><h1>{{title}}</h1>
    <p> {{body}}</p>
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
</style>





