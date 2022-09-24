<template>
  <div class="AddProjectFormC">
    <input type="text" v-model="project" placeholder="default" name="Project" id="Project">
    <div class="ButtonsContainer">
      <ProjectFormButton text="Add" btnclass="add" />
      <ProjectFormButton text="Cancel" btnclass="cancel" />
    </div>
  </div>
</template>

<script>

  import ProjectFormButton from './ProjectFormButton/ProjectFormButton.vue';

export default {
  name: 'AddProjectForm',
  components: {
    ProjectFormButton
  }
}
</script>

<style scoped>
  .ButtonsContainer {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>
