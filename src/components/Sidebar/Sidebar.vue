<template>
  <aside class="SidebarContainer">
    <SideMenuItem title="Inbox" classeIcon="fa-inbox" :active="InboxInitial" @click="ActiveClick('Inbox')"/>
    <SideMenuItem title="Today" classeIcon="fa-calendar-day" :active="TodayInitial" @click="ActiveClick('Today')" />
    <SideMenuItem title="Week" classeIcon="fa-calendar-week" :active="WeekInitial" @click="ActiveClick('Week')"/>
    <Projects />
  </aside>
</template>

<script>
  import SideMenuItem from './SideMenu/SideMenuItem.vue';
  import Projects from './SideMenu/Projects/Projects.vue';

export default {
  name: 'Sidebar',
  components: {
    SideMenuItem,
    Projects
  },
  data () {
    return {
      InboxInitial: true,
      TodayInitial: false,
      WeekInitial: false
    }
  },
  methods: {
    ActiveClick (element) {
      if (element === 'Inbox') {
        this.InboxInitial = true;
        this.TodayInitial = false;
        this.WeekInitial = false;
      } else if (element === 'Today') {
        this.InboxInitial = false;
        this.TodayInitial = true;
        this.WeekInitial = false;
      } else if (element === 'Week') {
        this.InboxInitial = false;
        this.TodayInitial = false;
        this.WeekInitial = true;
      }
    }
  }
}
</script>

<style scoped>
  .SidebarContainer {
   width: 15%;
   background-color: #32de84;
  }
 </style>
