<template>
  <div class="d-flex justify-center align-center" style="height: 90vh;">
    <v-card class="text-center" width="500" elevation="12">
      <v-icon size="100" class="mt-10">mdi-apple</v-icon>
      <v-card-text class="pa-10">

        <v-text-field 
        prepend-inner-icon="mdi-account" 
        variant="outlined" 
        label="Username"
        v-model="username"></v-text-field>
        <v-text-field 
        prepend-inner-icon="mdi-lock"
         variant="outlined" 
         label="Password"
         v-model="password" 
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
const username = ref ("")
const password = ref ("")

const defaultUsername = ref("admin")
const defaultPassword = ref("admin123")

function signIn(){
  //alert("Successfully signed in!");
  if(username.value === defaultUsername.value && password.value === defaultPassword.value){
    navigateTo("/dashboard");

  }else{
    alert("Invalid username or password. Please try again");
  }
}
</script>