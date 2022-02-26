<template>
  <notepad/>
</template>

<script>
  import notepad from '@/components/notepad';

export default {

  name: 'App',
  components: {
    notepad
  }
}
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
