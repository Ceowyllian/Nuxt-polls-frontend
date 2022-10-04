<template>
  <v-app dark>
    <TopNavigation />
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import TopNavigation from '../components/TopNavigation'

export default {
  name: 'DefaultLayout',
  components: { TopNavigation },
  data () {
    return {}
  }
}
</script>
