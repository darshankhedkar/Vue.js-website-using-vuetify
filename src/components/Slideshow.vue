<template>
<v-card class="mt-9" >
<v-carousel 
cycle hide-delimiter-background
 height="400" class="pb-1 ma-2">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      show-arrows-on-hover
       class="fill-height"
      
      href="/categories"
    ></v-carousel-item>
  </v-carousel>
</v-card>
  
</template>
<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://assets.myntassets.com/f_webp,w_980,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/17/189ec323-0590-45ac-a703-0a2ac9fde9e61637159055596-ggs_desktop.jpg',
          },
          {
            src: 'https://assets.myntassets.com/f_webp,w_980,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/15/45e4a12b-7249-41cf-82c3-9a14a52557581636989757162-Innerwear_Dk.jpg',
          },
          {
            src: 'https://assets.myntassets.com/f_webp,w_980,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/15/d1dc2223-8263-441e-90f6-828ab14efe1d1636990117280-The-Derma_Desk_Banner.jpg',
          },
          {
            src: 'https://assets.myntassets.com/f_webp,w_980,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/17/4813005f-09d4-46df-a0c5-d7258f24f9f81637161890088-Work-Wear_Desk.jpg',
          },
        ],
      }
    },
  }
</script>