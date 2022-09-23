<template>
  <Header />
  <Main />
</template>

<script>
  import Header from './views/Header.vue';
import Main from './views/Main.vue';

  export default {
    components: {
    Header,
    Main
}
  }

</script>

<style>

  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

    * {
      box-sizing: border-box;
      margin: 0px;
      padding: 0px;
    }

    html {
      font-family: 'Roboto', sans-serif;
    }

    .center {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100%;
    }
  </style>
