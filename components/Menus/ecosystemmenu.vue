<template>
  <v-row justify="center">
      <v-dialog v-model="dialog" :scrim="false" transition="dialog-bottom-transition">
          <template v-slot:activator="{ props }">
              <v-btn v-bind="props" class="rightAddBtn">
                  <v-icon start icon="fas fa-bars-staggered"></v-icon>
              </v-btn>
          </template>
          <v-card>
              <v-toolbar dark color="primary">
                  <v-btn icon dark @click="dialog = false">
                      <v-icon icon="fas fa-circle-xmark"></v-icon>
                  </v-btn>
                  <v-card-title>
                      <span class="text-h6">The Meeovi Company</span>
                  </v-card-title>
              </v-toolbar>
              <v-row style="padding: 10px;">
                  <v-col cols="3">
                      <a href="https://www.meeovi.com"><v-card class="mx-auto" width="200" prepend-icon="fas fa-shopping-cart">
                          <template v-slot:title>
                              Meeovi
                          </template>
                      </v-card></a>
                  </v-col>
              </v-row>
          </v-card>
      </v-dialog>
  </v-row>
</template>

<script>
  export default {
      data() {
          return {
              dialog: false,
              notifications: false,
              sound: true,
              widgets: false,
          }
      }
  }
</script>