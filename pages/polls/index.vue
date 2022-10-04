<template>
  <v-row>
    <v-col
      v-for="(question, i) in questions"
      :key="i"
      cols="12"
    >
      <QuestionCard :question="question" />
    </v-col>
  </v-row>
</template>

<script>
import QuestionCard from '../../components/QuestionCard'
export default {
  name: 'PollsPage',
  components: { QuestionCard },
  asyncData: async function () {
    const questions = []
    for (let i = 0; i < 10; i++) {
      questions.push({
        questionTitle: '#' + i,
        questionText: 'test text',
        pubDate: '01-10-2022',
        user: {
          username: 'John Doe',
          url: '#'
        }
      })
    }
    return await { questions }
  }
}
</script>
