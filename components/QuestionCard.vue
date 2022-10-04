<template>
  <v-lazy>
    <v-card
      elevation="5"
      nuxt
      to="#card"
    >
      <v-card-title>
        <div>{{ question.questionTitle }}</div>
        <v-chip
          outlined
          class="ms-auto"
          nuxt
          to="#"
        >
          <v-avatar
            color="grey darken-3"
            nuxt
            to="#"
          >
            <v-img
              alt=""
              src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
            />
          </v-avatar>
          <span class="ms-2">{{ question.user.username }}</span>
        </v-chip>
      </v-card-title>
      <v-card-subtitle>
        {{ question.pubDate }}
      </v-card-subtitle>
    </v-card>
  </v-lazy>
</template>

<script>

export default {
  name: 'QuestionCard',
  props: {
    question: {
      type: Object,
      default: null
    }
  },
  data: function () {
    return {}
  }
}
</script>

<style scoped>

</style>
