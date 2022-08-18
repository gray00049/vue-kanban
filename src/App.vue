<template>
  <div class="kanban-wrapper">

    <div class="kanban-board">
      <p class="kanban-board__title">Board 1</p>
      <div class="kanban-board__inner">
        <div class="kanban-board__task">
          Create kanban-board
        </div>
        <button class="kanban-board__add-new-task">+</button>
      </div>
    </div>

    <div class="kanban-board">
      <p class="kanban-board__title">Board 2</p>
      <div class="kanban-board__inner">
        <div class="kanban-board__task kanban-board__task--warning">
          Create kanban-board
        </div>
        <button class="kanban-board__add-new-task">+</button>
      </div>
    </div>

    <div class="kanban-board">
      <p class="kanban-board__title">Board 3</p>
      <div class="kanban-board__inner">
        <button class="kanban-board__add-new-task">+</button>
      </div>
    </div>

    <button class="kanban-board__add-new">+</button>

  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>
