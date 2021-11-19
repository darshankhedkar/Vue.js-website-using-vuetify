<template>
  <div class="mx-auto mb-5" max-width="500">
    <v-app-bar class="white" >
      
    
      <v-app-bar-title >Catogeries</v-app-bar-title>

      <v-spacer></v-spacer>
      
      <v-btn icon>
        <v-icon> mdi-heart-outline</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-shopping</v-icon>
      </v-btn>
    </v-app-bar>

    <v-list>
      <v-list-group 
        v-for="item in items"
        :key="item.title"
        v-model="item.active"
        :prepend-icon="item.action"
        no-action
      >
        <template v-slot:activator>
          <v-list-item-content class="white">
            <v-list-item-title  v-text="item.title"></v-list-item-title>

          </v-list-item-content>
        </template>

        <v-list-item  v-for="child in item.items" :key="child.title">
          <v-list-item-content>
            
            <v-list-item-title v-text="child.title"></v-list-item-title> 
          </v-list-item-content>
        </v-list-item>
      </v-list-group>
    </v-list>
    
    <v-list-content> </v-list-content>
  </div>
  
</template>
<script>
export default {
  data: () => ({
   
    items: [
      {
        action: "mdi-ticket",
        items: [
          { title: "Brands" },
          {title:"Indian & Fusion Wear"},
          {title:"Western Wear"},
          {title:"Lingerie & Sleepwear"},
          {title:"Footwear"},
          {title:"Sports & Active Wear"},
          {title:"Handbags,Bags & Wallets"},
          {title:"Watches"},
          {title:"Sunglasses & Frames"},
          {title:"Cosmetics & Personal Care"},
          {title:"Headphones & Speakers"},
          {title:"Jewellery"},
          {title:"Accessories"},
          {title:"Luggage & Trolleys"},


        ],
        title: "WOMEN",
      },
      {
        action: "mdi-silverware-fork-knife",

        items: [
          { title: "Brands" },
          {title:"TopWear"},
          {title:"BottomWear"},
          {title:"Sports & Active Wear"},
          {title:"Inner & Sleepwear"},
          {title:"Indian & Festive Wear"},
          {title:"Suits & Blazers"},
          {title:"Plus Size"},
          {title:"Footwear"},
          {title:"Watches"},
          {title:"Personal Care & Grooming"},
          {title:"Headphones & Speakers"},
          {title:"Bags & Bagpacks"},
          {title:"Luggage & Trolleys"},
          {title:"Accessories"},
        ],
        title: "MEN",
      },
      {
        action: "mdi-school",
        items: [
          { title: "Brands" },
          { title: "Boys Clothing" },
          { title: "Girls Clothing" },
          { title: "Boys Footwear" },          
          { title: "Girls Footwear" },
          { title: "Kids Accessories" },
          { title: "Toys" },
          ],
        title: "KIDS",
      },
      {
        action: "mdi-run",
        items: [
          { title: "Explore Home Store" },
          { title: "Gifting ideas" },
          { title: "Brands" },
          { title: "Bed Linen & Furnishing" },
          { title: "Curtains" },
          { title: "Cushions & Cushion Covers" },
          { title: "Home Decor" },
          { title: "Lamps & Lighting" },
          { title: "Flooring" },
          { title: "Bath" },
          { title: "kitchen & Table" },
          { title: "Storage" },
          ],
        title: "Home",
      },
      {
        action: "mdi-bottle-tonic-plus",
        items: [
          { title: "Explore Audio Store" },
          { title: "Headphones" },
          { title: "Speakers" },
          { title: "Explore Travel Store" },
          { title: "Trollys" },
          { title: "Rucksacks" },
          ],
        title: "GADGETS",
      },
     
    ],
  }),
};
</script>