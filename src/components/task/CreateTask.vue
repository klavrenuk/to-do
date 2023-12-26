<template>
  <div class="create_task">
    <div class="create_task__header">
      <input
          class="create_task__input w-full todo_input"
          placeholder="Add a task"
      />
    </div>
    <div class="create_task__control flex justify-end">
      <button class="create_task__add todo_btn">add</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
$padding: .5rem;

.create_task {
  &__input {
    padding: 3px $padding;
  }

  &__control {
    padding: 3px $padding;
    background: rgba(204,204,204, .3);
  }
}
</style>
