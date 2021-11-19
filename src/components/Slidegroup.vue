<template>
<div>
  <div>
    <v-card flat class="pa-8">
      <h2>DEALS OF THE DAY</h2>
    </v-card>
  </div>
<v-container  >
    <v-row >
      <v-col v-for="card in cards" :key="card.id" :cols="auto">
        <v-card >
          <v-img :src="card.src" width="213px" height="330px">
            
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</div>
  
</template>
<script>
export default {
  data: () => ({
    cards: [
      {
        src: "https://assets.myntassets.com/f_webp,w_196,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/17/3871989a-a4fb-4ed2-b678-0c1f4d00c28d1637144634381-B1A799.jpg",
      },
      {
        src: "https://assets.myntassets.com/f_webp,w_196,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/16/1b85367c-c042-43c7-ace9-7cff3e278c4d1637074953073-Kurta-Sets.jpg",
      },
      {
        src: "https://assets.myntassets.com/f_webp,w_196,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/16/911f167d-5234-4fcc-a142-d8ec961055fe1637074953081-Winter-Wear.jpg",
      },
      {
        src: "https://assets.myntassets.com/f_webp,w_196,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/16/b4af7620-b167-4c37-9f9f-b35749d1ca5f1637074953057-Winter-Boots.jpg",
      },
      {
        src: "https://assets.myntassets.com/f_webp,w_196,c_limit,fl_progressive,dpr_2.0/assets/images/2021/11/16/951eed39-19c5-4de6-a16a-37ba56bc729b1637076400891-DYSON.jpg",
      },
      
    ],
  }),
};
</script>