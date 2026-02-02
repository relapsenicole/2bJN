<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" :rail="rail" permanent="">
      <template v-slot:prepend>
        <v-list-item
          lines="two"
          prepend-avatar="https://th.bing.com/th/id/OIP.eV2p-CGFxIff8EmZxacNxgHaFg?o=7rm=3&rs=1&pid=ImgDetMain&o=7&rm=3"
          subtitle="Logged in"
          title="cat cat"
        ></v-list-item>
      </template>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item
          prepend-icon="mdi-home-city"
          title="Home"
          value="home"
        ></v-list-item>
        <v-list-item
          prepend-icon="mdi-account"
          title="My Account"
          value="account"
        ></v-list-item>
        <v-list-item
          prepend-icon="mdi-account-group-outline"
          title="Users"
          value="users"
        ></v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :elevation="2">
      <template v-slot:prepend>
        <v-app-bar-nav-icon @click="rail = !rail"></v-app-bar-nav-icon>
      </template>

      <v-app-bar-title>Application Bar</v-app-bar-title>
    </v-app-bar>
    <v-main>
      <v-container fluid>
        <slot />
      </v-container>
    </v-main>
  </v-app>
  
</template>


<script setup>
const drawer = ref(true)
const rail = ref(false)
</script>

<style>
</style>