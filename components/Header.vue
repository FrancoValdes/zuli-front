<template>
  <div>
    <b-navbar class="justify-content-end" type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item
          v-for="(title, index) in titles"
          :key="index"
          :href="title.to"
          >{{ title.name }}</b-nav-item
        >
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      titles: [
        {
          name: 'Inicio',
          to: '/'
        },
        {
          name: 'Acerca de Nosotros',
          to: 'acerca-de-nosotros'
        },
        {
          name: 'Contacto',
          to: '/contacto'
        }
      ]
    }
  }
}
</script>

<style></style>
