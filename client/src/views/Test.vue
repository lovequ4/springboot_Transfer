<template>
 
    
      <q-btn label="Medium" color="primary" @click="medium = true" />
     
  
     
      <q-dialog
        v-model="medium"
      >
        <q-card style="width: 700px; max-width: 80vw;">
          <q-card-section>
            <div class="text-h6">Medium</div>
          </q-card-section>
  
          <q-card-section class="q-pt-none">
            Click/Tap on the backdrop.
          </q-card-section>
  
          <q-card-actions align="right" class="bg-white text-teal">
            <q-btn flat label="OK" v-close-popup />
          </q-card-actions>
        </q-card>
      </q-dialog>
  
    
  </template>
  
  <script>
  import { ref } from 'vue'
  
  export default {
    setup () {
      return {
        small: ref(false),
        medium: ref(false),
        fullWidth: ref(false),
        fullHeight: ref(false)
      }
    }
  }
  </script>