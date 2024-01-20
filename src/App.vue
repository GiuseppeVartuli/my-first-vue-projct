<script>
export default {
  name: "App",
  data() {
    return {
      message: "Giuseppe",
      background: "purple",
      movie: "",
    };
  },
  methods: {
    greetings() {
      console.log("ciao", this.message);
    },
  },
};
</script>

<template>
  <h1 :class="background">{{ message }}</h1>
  <button v-on:click="greetings">Cliccami</button>

  <label for="movie">Movie</label>
  <input type="text" id="movie" v-model="movie" />

  <p>{{ movie }}</p>
</template>

<style></style>
