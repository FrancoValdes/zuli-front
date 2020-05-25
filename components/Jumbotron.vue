<template>
  <div>
    <b-jumbotron
      bg-variant="light"
      text-variant="primary"
      border-variant="black"
      header-level="3"
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
      title: 'Imperio Lapizlázuli',
      subtitle: 'Artesanias y Joyeria '
    }
  }
}
</script>

<style></style>
