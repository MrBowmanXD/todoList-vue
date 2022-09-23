<template>
  <main class="MainContainer">
    <Sidebar />
    <MainArea />
  </main>
</template>

<script>

  import Sidebar from '../components/Sidebar/Sidebar.vue';
  import MainArea from '../components/MainArea/MainArea.vue';

export default {
  name: 'Main',
  components: {
    Sidebar,
    MainArea
  }
}
</script>

<style scoped>
  .MainContainer {
    display: flex;
    height: 80vh;
  }
</style>