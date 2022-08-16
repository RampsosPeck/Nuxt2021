<template>
  <div class="details">
    <p>{{posts.id}}</p>
    <h1>{{posts.title}}</h1>
    <p>{{posts.body}}</p>
  </div>
</template>

<script>

const url = "https://jsonplaceholder.typicode.com/posts/";

import axios from "axios";

export default {
  asyncData({$axios, route}){
    return $axios.get(url + route.params.id).then(res =>{
      return {posts: res.data};
    })
  },
  data(){
    return {};
  }
}
</script>



<style scoped>
.details{
  border: 1px solid black;
  padding: 10px;
  margin: 20px;
}
</style>
