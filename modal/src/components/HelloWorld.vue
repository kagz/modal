<template>
  <v-container>
    <v-layout row justify-center>
      <v-dialog v-model="dialog" persistent max-width="290">
        <v-btn slot="activator" color="primary" dark>Click Me </v-btn>
        <v-card>
          <v-card-title class="headline">THIS IS A MODAL POP-UP</v-card-title>
          <v-card-text>Nothing happens until is closed </v-card-text>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn color="green darken-1" flat @click="dialog = false">Yes</v-btn>
            <v-btn color="green darken-1" flat @click="dialog = false">Nope</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false
      }
    }
  }
</script>
