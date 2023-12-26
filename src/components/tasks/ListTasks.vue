<script setup lang="ts">
import {PropType} from 'vue';
import CardTask from "@/components/task/CardTask.vue";

import {ITask} from "@/interfaces/Task";

const {tasks} = defineProps({
  tasks: {
    type: Array as PropType<ITask[]>,
    required: false,
    default: []
  }
});
</script>

<template>
  <div class="list_tasks">
    <CardTask
        v-for="task in tasks"
        :key="task.id"
        :task="task"
    />
  </div>
</template>
