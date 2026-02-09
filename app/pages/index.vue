<template>
  <div>
    <h1>Welcome To My Nuxt App</h1>
  </div>

  <v-row>
    <v-col cols="12" md="3">
      <v-card height="150" color="black">
        <v-card-text>
          <v-row no-gutter>
            <v-col cols="6">
              <v-icon size="100">mdi-currency-usd</v-icon>
            </v-col>
            <v-col cols="6">
              <v-row>
                <v-col cols="12" class="text-h4 text right">STUDENT</v-col>
                <v-col cols="12" class="text-h3 text center">250</v-col>
              </v-row>
            </v-col>
          </v-row>
        </v-card-text>
      </v-card>
    </v-col>

    <v-col cols="12" md="3">
      <v-card height="150" color="blue"></v-card>
    </v-col>
    <v-col cols="12" md="3">
      <v-card height="150" color="green"></v-card>
    </v-col>
    <v-col cols="12" md="3">
      <v-card height="150" color="yellow"></v-card>
    </v-col>
    <v-col cols="12" md="3">
      <v-card height="150" color="pink"></v-card>
    </v-col>
    <v-col cols="12" md="3">
      <v-card height="150" color="black"></v-card>
    </v-col>
  </v-row>
</template>
<script lang="ts" setup>
</script>

<style>
</style>