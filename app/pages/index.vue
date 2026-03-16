<template>
  <div class="d-flex justify-center align-center" style="height: 90vh;">
    <v-card class="text-center" width="500" elevation="12">
      <v-icon size="100" class="mt-10">mdi-apple</v-icon>
      <v-card-text class="pa-10">

        <v-text-field 
        prepend-inner-icon="mdi-account" 
        variant="outlined" 
        label="Username"></v-text-field>
        <v-text-field 
        prepend-inner-icon="mdi-lock"
         variant="outlined" 
         label="Password" 
         type="password"></v-text-field>
         <v-btn block color="black" @click="signIn">Sign in</v-btn>
      </v-card-text>
    </v-card>
  </div>
</template>
<script setup>
definePageMeta({
  layout: "auth"
}

);

function signIn(){
  alert("Successfully signed in!");
}
</script>