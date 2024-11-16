<template>
  <div
    @dblclick="$emit('toggle-reminder', task.id)"
    :class="[task.reminder ? 'reminder' : '', 'task']"
  >
    <h3>
      {{ task.text }}
      <i @click="$emit('delete-task', task.id)" class="fas fa-times"></i>
    </h3>

    <p>{{ task.day }}</p>
  </div>
</template>

<script>
export default {
  name: "MyTask",
  props: {
    task: Object,
  },
};
</script>
<style scope>
.fas {
  color: rgb(255, 0, 0);
}
.task {
  background: rgb(244, 244, 244);
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
  border-radius: 5px;
  box-shadow: 0 4px 12px rgb(62, 63, 62);
}

.task.reminder {
  border-left: 5px solid rgb(0, 128, 0);
}

.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
