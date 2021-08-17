<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <h2 class="timer">{{ time }}</h2>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data() {
    return {
      time: 1,
    }
  },
  components: {
    HelloWorld,
  },
  methods: {
    add() {
      if (this.time == 1) {
        this.time = 2
      }
    },
  },
}
</script>
<style lang="scss" scoped>
.home {
  .timer {
    background: #f40;
  }
}
</style>
