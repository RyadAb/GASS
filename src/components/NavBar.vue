<template>
    <div>
        <v-app-bar
      app
      color="deep-purple accent-4"
      dark
      flat
    >
      
      <img class="mr-3" :src="require('../assets/gass.png')" height="45"/>

      <v-toolbar-title>GASS</v-toolbar-title>

      <v-spacer></v-spacer>
      
      <v-toolbar-items>
        <v-btn
          text
          flat
          v-for="item in navItems"
          :key="item.title">
          {{ item.title }}
        </v-btn>
      </v-toolbar-items>

      <v-text-field    
        style="width: 0px"
        class="mx-4"
        flat
        hide-details
        label="Search"
        prepend-inner-icon="search"
        solo-inverted
      ></v-text-field>

      <v-divider
      light
      vertical
      inset
      ></v-divider>

      <v-btn text @click="dialog = true">Sign in</v-btn>
    </v-app-bar>

    <v-row no-gutters>
    <v-dialog v-model="dialog" max-width="1000px">
      <Sign/>
    </v-dialog>
  </v-row>

    </div>
</template>


<script>
import Sign from './Sign.vue'
export default {
    components: {
        Sign
    },
    data() {
        return {
        navItems:[
            {title: 'Home'},
            {title: 'Contacts'},
            {title: 'Sitemap'},
        ],
        dialog: false,
        }
    },
}
</script>