<template>
<v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      :src="image"
    >
      <v-card-title>{{ title }}</v-card-title>
    </v-img>

    <v-card-subtitle class="pb-0">{{ author }}</v-card-subtitle>

    <v-card-text class="text--primary">
      <div>{{ description }}</div>
    </v-card-text>
<!--
    <v-card-actions>
      <v-btn
        color="orange"
        text
      >
        Explore
      </v-btn>
    </v-card-actions>
-->
  </v-card>

</template>
<script>
export default {
      props: ['author', 'image', 'title', 'description']
}
</script>