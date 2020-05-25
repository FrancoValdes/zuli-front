<template>
  <div class="container-fluid">
    <Header />
    <Jumbotron />
    <section>
      <Card
        v-for="(item, index) in items"
        :key="index"
        :image="item.image"
        :name="item.name"
        :description="item.description"
      />
    </section>
  </div>
</template>

<script>
import Jumbotron from '~/components/Jumbotron'
import Header from '~/components/Header'
import Card from '~/components/Card'

export default {
  components: {
    Jumbotron,
    Header,
    Card
  },
  data() {
    return {
      items: [
        {
          name: 'Collar lapizlázuli one',
          description:
            'Hecho de acero quirurjico y lapizulázuli pulido con tratamiento de brillo, 24 gramos',
          image: '',
          to: ''
        },
        {
          name: 'Elefante de cuarso',
          description:
            'Figura de elefante en piedra tallada. Amuleto, Cuarzo rosa, 1. 300 gramos',
          image: '',
          to: ''
        }
      ]
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
