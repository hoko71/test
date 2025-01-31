<template>
  <Modal/>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: "App",
  components: { Modal },
  data() {
    return {
      title: "this is test",
    };
  },
  methods: {
    handleEvent() {
      console.log("event");
      console.log(this.$refs.name);
      this.$refs.name.classList.add("mahdi");
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
