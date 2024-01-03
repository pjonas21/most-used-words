<template>
  <v-container fluid>
    <div class="pills">
      <PillWord v-for="word in groupWords" :key="word.name" :name="word.name" :amount="word.amount" />
    </div>
  </v-container>
</template>

<script>
import PillWord from './PillWord.vue'

export default {

  components: {
    PillWord,
  },

  data: function () {
    return {
      groupWords: [
        { name: 'you', amount: 900},
        { name: 'he', amount: 760},
        { name: 'i', amount: 1342},
      ]
    }
  }

}
</script>

<style>

</style>