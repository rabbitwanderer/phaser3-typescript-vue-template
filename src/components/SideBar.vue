<template>
  <div class="d-flex flex-column ma-2">
    <v-btn small @click="stop()">Stop</v-btn>
    <span>{{ x }}</span>
    <span>{{ y }}</span>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import store from '@/store'

export default {
  name: 'SideBar',
  data() {
    return {
    }
  },
  computed: {
    ...mapState(['x', 'y'])
  },
  methods: {
    stop() {
      store.dispatch('stop');
    }
  }
}
</script>

<style lang="scss" scoped>
</style>
