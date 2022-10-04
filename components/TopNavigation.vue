<template>
  <v-app-bar
    app
    clipped-left
    dense
    fixed
  >
    <v-toolbar-title class="col">
      <v-btn nuxt to="/" color="primary">
        <v-icon class="me-2">
          mdi-home
        </v-icon>
        Django polls
      </v-btn>
    </v-toolbar-title>
    <v-text-field
      append-icon="mdi-search-web"
      class="mt-6 col-8"
      clearable
      dense
      solo-inverted
    />
    <v-col>
      <div class="float-end">
        <v-btn nuxt to="account">
          <v-icon>mdi-account</v-icon>
        </v-btn>
        <v-btn nuxt to="about">
          <v-icon>mdi-information-outline</v-icon>
        </v-btn>
      </div>
    </v-col>
  </v-app-bar>
</template>

<script>
export default {
}
</script>

<style scoped>

</style>
