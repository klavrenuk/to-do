<script setup lang="ts">
import CreateTask from "@/components/task/CreateTask.vue";
import ListTasks from "@/components/tasks/ListTasks.vue";

import {ITask} from "@/interfaces/Task";

const tasks:ITask[] = [
  {
    id: 1,
    name: 'name',
    isChecked: false,
    description: 'description',
    subTasks: []
  },
  {
    id: 2,
    name: 'name#2',
    isChecked: false,
    description: 'description',
    subTasks: []
  },
  {
    id: 3,
    name: 'name#3',
    isChecked: false,
    description: 'description',
    subTasks: []
  }
];
</script>

<template>
  <div class="category_view">
    <h2 class="category_view__title mb-5">Title</h2>

    <div class="category_view__create mb-2">
      <CreateTask />
    </div>

    <ListTasks :tasks="tasks" />
  </div>
</template>

<style scoped lang="scss">
.category_view {
  &__title {
    color: #0066FF;
    font-size: 18px;
  }
}
</style>
