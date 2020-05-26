<template>
  <div>
    <b-card
      :title="name"
      :img-src="image ? image : 'https://picsum.photos/600/300/?image=25'"
      img-alt="Image"
      img-top
      tag="article"
      style="max-width: 20rem;"
      class="mb-2"
    >
      <b-card-text>
        {{ description }}
      </b-card-text>
      <!-- <b-button :href="to? to : '#'" variant="primary"></b-button> -->
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: ['name', 'description', 'image', 'to']
}
</script>

<style></style>
