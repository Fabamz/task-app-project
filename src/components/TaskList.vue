<template>
  <div>
    <div v-for="task in tasks" :key="task.id">
      <MyTask
        @toggle-reminder="$emit('toggle-reminder', task.id)"
        @delete-task="$emit('delete-task', task.id)"
        :task="task"
      />
    </div>
  </div>
</template>

<script>
import MyTask from "./MyTask.vue";

export default {
  name: "TaskList",
  props: {
    tasks: Array,
  },
  components: {
    MyTask,
  },
  emits: ["delete-task", "toggle-reminder"],
};
</script>
