<template>
  <v-app>
    <v-app-bar flat>
      <v-app-bar-title>
        電子公告 | bitboxx
      </v-app-bar-title>
    </v-app-bar>
    <v-main>
      <router-view/>
    </v-main>
    <v-footer app>
      2024 &copy; bitboxx Inc.
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',

  data () {
    return {
      //
    }
  },
})
</script>
