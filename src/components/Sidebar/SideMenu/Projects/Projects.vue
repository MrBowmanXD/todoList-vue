<template>
    <ProjectsTitle />
    <AddProject />
  </template>

  <script>
    import ProjectsTitle from './ProjectsTitle.vue';
    import AddProject from './AddProject.vue';

  export default {
    name: 'Projects',
    components: {
      ProjectsTitle,
      AddProject
    }
  }
  </script>

  <style scoped>
  </style>
