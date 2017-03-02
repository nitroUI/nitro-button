<template>
  <button v-on:click="showAlert">{{text}}</button>
</template>

<script>
export default {
  props: ['text', 'alert'],
  data () {
    return {
    }
  },
  methods: {
    showAlert: function() {
      if (this.alert) {
        alert('Hello! Buttercup!');
      }
    }
  }
}
</script>

<style lang="scss">
nitro-button {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
