<template>
<v-app>
  <div class="d-flex flex-row ma-2">
    <v-card tile>
      <SideBar />
    </v-card>
    <v-card tile>
      <Game />
    </v-card>
  </div>
</v-app>
</template>
<script lang="ts">
import Game from '@/components/Game.vue'
import SideBar from '@/components/SideBar.vue'

export default {
  name: 'App',
  components: { Game, SideBar }
}
</script>

<style lang="scss">
body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
}
</style>
