<template>
  <div class="container">
    <Jumbotron />
  </div>
</template>

<script>
import Jumbotron from '~/components/Jumbotron.vue'

export default {
  components: {
    Jumbotron
  },
  data() {
    return {
      items: [0, 1, 2, 3, 4]
    }
  }
}
</script>

<style scoped>
.flexContainer {
  text-align: center;
}

.flexItem {
  width: 100px;
  height: 100px;
  background: orange;
  text-align: center;
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
