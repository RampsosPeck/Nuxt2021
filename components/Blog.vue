<template>
	<div class="main_item">
    <div class="images" :style="{backgroundImage: 'url('+img+')'}">

    </div>
		<h1>{{title}}</h1>
		<p>{{des}}</p>
	</div>
</template>

<script>
export default{
	props:["title","des", "img"]

}
</script>

<style scoped>
.main_item{
  height:300px;
  width: 300px;
  background-color: crimson;
  padding: 10px;
  margin: 10px;
  color: aliceblue;
  border-radius:20px;

}

.images {
  background-position: center;
  background-size: cover;
  height: 200px;
  width: 280px;
  margin: 10px;
  border-radius:20px;
}

</style>

