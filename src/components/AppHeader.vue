<template>
  <header>
    <h1>{{ title }}</h1>
    <CustomButton
      v-show="homepage"
      @btn-click="$emit('toggle-add-task')"
      :text="showAddTask ? 'close' : 'Add Task'"
      :color="showAddTask ? 'red' : 'green'"
    />
  </header>
</template>

<script>
import CustomButton from "./CustomButton.vue";

export default {
  name: "AppHeader",
  props: {
    title: String,
    showAddTask: Boolean,
  },
  components: {
    CustomButton,
  },
  computed: {
    homepage() {
      if (this.$route.path === "/") {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}

h1 {
  margin-right: 30px;
}
</style>
