<template>
  <v-app id="inspire">
    <v-navigation-drawer :width="226" v-model="drawer" app>
      <v-list-item title="My Application" subtitle="Vuetify">Application</v-list-item>
      <v-divider></v-divider>
      <v-list-item link title="List Item 1"></v-list-item>
      <v-list-item link title="List Item 2"></v-list-item>
      <v-list-item link title="List Item 3"></v-list-item>
    </v-navigation-drawer>
    
    <v-app-bar app>
      <v-btn @click="alerta()">hi</v-btn>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>
  </v-app>
</template>


<script>
export default {
  data: () => ({
     drawer: null }),
  methods:{
    alerta(){
      alert('hihi');

    }
  }
}

</script>