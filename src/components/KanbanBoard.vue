<template>
  <div class="kanban-board">
    <p class="kanban-board__title">{{ board.title }}</p>
    <div class="kanban-board__inner">
      <div 
        class="kanban-board__task" 
        :class="{
          'kanban-board__task--done': task.status == 'done',
          'kanban-board__task--warning': task.importance == 'high',
        }" 
        v-for="(task, id) in board.tasks" 
        :key="id"
      >
        {{ task.text }}
      </div>
      <button class="kanban-board__add-new-task">+</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'KanbanBoard',
  props: [ 'board' ]
}
</script>
