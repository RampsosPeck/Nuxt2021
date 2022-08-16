<template>
  <div class="main_blog">
    <BlogPortal
      v-for="post in data" :key="post.id"
      :title="post.title"
      :body="post.body"
      :id="post.id"
    />
  </div>
</template>

<script>

import BlogPortal from '../../components/BlogPortal.vue';

const url = "https://jsonplaceholder.typicode.com/posts";

import axios from 'axios';

export default {

  components:{
    BlogPortal,
  },
  data(){
    return {
      data:[]
    }
  },
  mounted(){
    axios.get(url)
    .then(res=>{
      this.data = res.data
    }).catch(err =>{
      console.log(err);
    })
  }

}
</script>



