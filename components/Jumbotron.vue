<template>
  <div>
    <b-jumbotron
      bg-variant="light"
      text-variant="primary"
      border-variant="black"
    >
      <template v-slot:header>{{ title }}</template>

      <template v-slot:lead>
        {{ subtitle }}
      </template>

      <hr class="my-4" />
      <b-button variant="success" href="#">Ver mas</b-button>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  name: 'Jumbotron',
  data() {
    return {
      title: 'Imperio Lapizlazuli',
      subtitle: 'Artesanias y Joyeria '
    }
  }
}
</script>

<style></style>
