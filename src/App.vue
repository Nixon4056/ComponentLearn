<template>
  <div>
    <the-header></the-header>
    <button>Active goals</button>
    <button>Manage goals</button>
    <active-goals></active-goals>
    <manage-goals></manage-goals>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
/* import BadgeList from './components/BadgeList.vue';
import UserInfo from './components/UserInfo.vue';
import CourseGoals from './components/CourseGoals.vue'; */
import ActiveGoals from './components/ActiveGoals.vue';
import ManageGoals from './components/ManageGoals.vue';

export default {
  components: {
    'the-header': TheHeader,
    'manage-goals': ManageGoals,
    'active-goals': ActiveGoals
  },
  data() {
    return {
      activeUser: {
        name: 'Maximilian Schwarzmüller',
        description: 'Site owner and admin',
        role: 'admin',
      },
    };
  },
};
</script>

<style>
html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>