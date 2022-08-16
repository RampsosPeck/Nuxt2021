<template>
  <div class="portal">
    <h3>{{title}}</h3>
    <p>{{des}}</p>
    <div class="images" :style="{backgroundImage:'url('+img+')'}"></div>
  </div>
</template>

<script>

export default{
  props: ["title","des", "img"]
}

</script>

<style scoped>
.portal {
  height: 500px;
  width: 50%;
  margin: 10px;
  align-items: center;
  text-align: center;
  background-color: chartreuse;
}
.images{
  background-position: center;
  background-size: cover;
  height: 400px;
  width: 100%;
  border-radius: 20px;
}
</style>
