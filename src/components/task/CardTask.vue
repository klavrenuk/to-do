<script setup lang="ts">
import {ITask} from "@/interfaces/Task";

const {task} = defineProps({
  task: {
    type: ITask,
    required: true
  }
});
</script>

<template>
  <div class="card_task">
    {{ task.name }}
  </div>
</template>
