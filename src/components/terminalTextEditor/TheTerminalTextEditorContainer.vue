<template>   
  <button @click="setDisplay">Toggle</button>
  <!-- <TheTerminal v-show="showTerm"/> -->
  <TheTextEditor v-show="showText"/>
</template>

<script>
// Due to issues with terminal, temporarily commented out
// import TheTerminal from './TheTerminal.vue';
import TheTextEditor from './TheTextEditor.vue';

export default {
  components: {
    // TheTerminal,
    TheTextEditor,
  },
  data() {
    return {
      showTerm: false,
      showText: true,
    }
  },
  methods: {
    setDisplay() {
      this.showTerm = !this.showTerm;
      this.showText = !this.showText;
    }
  }
}
</script>

<style scoped>
  
</style>