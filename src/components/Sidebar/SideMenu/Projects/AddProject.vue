<template>
  <div class="ContainerProject" @click="AddProjectClicked">
    <i class="fa-solid fa-plus"></i>
    <h4>Add Project</h4>
  </div>
  <div v-if="AddProject" class="AddProjectFormContainer">
    <AddProjectForm />
  </div>

</template>

<script>
  import AddProjectForm from './AddProjectForm/AddProjectForm.vue';

export default {
  name: 'AddProject',
  components: {
    AddProjectForm
  },
  data () {
    return {
      AddProject: false,
    }
  },
  methods: {
    AddProjectClicked() {
      this.AddProject = true;
    }
  }
}
</script>

<style scoped>
 .ContainerProject {
  display: flex;
  align-items: center;
  padding: 15px;
  cursor: pointer;
 }

 .ContainerProject:hover {
      background-color: #1CAC78;
    }
    .ContainerProject h4 {
      font-weight: 300;
      font-size: 24px;
    }

 .fa-solid {
      margin-right: 15px;
    }
</style>
