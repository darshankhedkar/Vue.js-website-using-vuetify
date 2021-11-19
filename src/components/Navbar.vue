<template>
  <div>
    <v-navigation-drawer v-model="drawer" app>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6 text-uppercase">
            Mantra
          </v-list-item-title>
          <v-list-item-subtitle class="text-capitalize">
            Become inside
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list nav>
        <v-list-item v-for="item in items" :key="item.title" link :to="item.to">
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app class="white" flat >
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title >
        <v-img  height="60px" width="80px"
        src="https://gumlet.assettype.com/afaqs%2F2021-01%2F15f5f827-8e29-4520-af8d-a0f353b8da17%2Fimages.png?">

        </v-img>
       
      </v-toolbar-title>
       <v-card-title class="text-uppercase" flat>
        become outstanding
        </v-card-title>
      <v-spacer></v-spacer>
      <v-toolbar-content>
        
        <v-text-field
          v-model="message2"
          solo
          label="Search"
          clearable
          class="pt-10"
          outlined
          flat
        >
        
        </v-text-field>
        
      </v-toolbar-content>
    </v-app-bar>
  </div>
</template>


<script>
export default {
  data() {
    return {
      drawer: false,
      items: [
        { title: "Home", icon: "mdi-home", to: "/" },
        { title: "Categories", icon: "mdi-eye-arrow-right-outline", to: "/categories" },
        { title: "Profile", icon: "mdi-google-street-view", to: "/profile" },
      ],
    };
  },
};
</script>