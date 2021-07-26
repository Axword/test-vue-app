<template>
  <div class="text-center">
    <v-col>
      <v-btn @click="addscoreForPlayerOne" test rounded color="primary" dark>Rounded Button</v-btn>
      <span>Player1 {{ scoreForPlayerOne }}</span>
    </v-col>
    <v-col>
      <v-btn @click="addscoreForPlayerTwo" test rounded color="primary" dark>Rounded Button</v-btn>    
      <span>Player2 {{ scoreForPlayerTwo }}</span>
    </v-col>
  </div>
</template>

<script>
export default {
  data() {
    return {
        scoreForPlayerOne: 1,
        scoreForPlayerTwo: 1,
      }
  },
  methods: {
    addscoreForPlayerOne() {
      this.scoreForPlayerOne = ++this.scoreForPlayerOne;
    },
    addscoreForPlayerTwo() {
      this.scoreForPlayerTwo = ++this.scoreForPlayerTwo;
    }
  }
}
</script>
