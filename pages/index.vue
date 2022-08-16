<template>
  <!--<Tutorial/>-->
  <div>

    <div class="top_main">
      <Blog title="Nuxt JS" des="Nosotros aprehendemos Nuxt"
        img="https://images.fineartamerica.com/images/artworkimages/medium/1/all-you-need-is-love-balazs-solti.jpg"
      />
      <Blog title="Nuxt REACT" des="Nosotros aprehendemos REACT"
        img="https://render.fineartamerica.com/images/rendered/search/phone-case/iphone13/images-medium-5/hummingbird-of-watercolor-rainbow-olga-shvartsur.jpg?&targetx=0&targety=108&imagewidth=593&imageheight=771&modelwidth=564&modelheight=988&backgroundcolor=FFFFFF&orientation=0&producttype=iphone13"
      />
      <Blog title="Nuxt VUE" des="Nosotros aprehendemos VUE"
        img="https://render.fineartamerica.com/images/rendered/search/phone-case/iphone13/images-medium-5/2-on-our-way-ryan-hartson-weddle.jpg?&targetx=-34&targety=0&imagewidth=651&imageheight=988&modelwidth=564&modelheight=988&backgroundcolor=0C0B0E&orientation=0&producttype=iphone13"
      />
      <Blog title="Nuxt VUE" des="Nosotros aprehendemos VUE"
        img="https://render.fineartamerica.com/images/rendered/search/phone-case/iphone13/images/artworkimages/medium/1/the-dreamer-martine-roch.jpg?&targetx=0&targety=-200&imagewidth=988&imageheight=988&modelwidth=988&modelheight=564&backgroundcolor=28455B&orientation=1&producttype=iphone13"
      />
      <Blog title="Nuxt REACT" des="Nosotros aprehendemos REACT"
        img="https://render.fineartamerica.com/images/rendered/search/phone-case/iphone13/images-medium-5/hummingbird-of-watercolor-rainbow-olga-shvartsur.jpg?&targetx=0&targety=108&imagewidth=593&imageheight=771&modelwidth=564&modelheight=988&backgroundcolor=FFFFFF&orientation=0&producttype=iphone13"
      />
    </div>
    <div class="portal_section">
      <Portal title="Nuevo dpocumental" des="Casi por siempre terminado"
        img="https://render.fineartamerica.com/images/rendered/search/phone-case/iphone13/images-medium-5/hummingbird-of-watercolor-rainbow-olga-shvartsur.jpg?&targetx=0&targety=108&imagewidth=593&imageheight=771&modelwidth=564&modelheight=988&backgroundcolor=FFFFFF&orientation=0&producttype=iphone13"
      />
      <Portal title="Nuevo dpocumental" des="Casi por siempre terminado"
        img="https://images.fineartamerica.com/images/artworkimages/medium/1/all-you-need-is-love-balazs-solti.jpg"
      />
    </div>
  </div>
</template>

<script>
import Blog from "../components/Blog.vue";
import Portal from "../components/Portal.vue";


export default {
  components:{
    Blog,
    Portal
  },
  head(){
    return {
      titleTemplate: '%s - Nuxtjs',
      meta: [
        { charset: 'utf-8' },
        { name: 'viewport', content: 'width=device-width, initial-scale=1' },

        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: 'Meta description' }
      ]
    }
  }
}


</script>

<style>

.top_main{
  display:flex;
}
.portal_section{
  display:flex;
}
</style>


