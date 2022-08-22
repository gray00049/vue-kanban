<template>
  <div class="kanban-wrapper">
    
    <KanbanBoard v-for="(board, id) in boards" :key="id" :board="board" />

    <button class="kanban-board__add-new">+</button>

  </div>
</template>

<script>
import KanbanBoard from "@/components/KanbanBoard.vue";
export default {
  name: "App",
  data() {
    return {
      boards: [
        {
          title: "My task",
          tasks: [
            {
              status: "inwork",
              importance: "ordinary",
              text: "Create kanban board"
            },
            {
              status: "done",
              importance: "ordinary",
              text: "Create start template"
            },
          ]
        },
        {
          title: "Other task",
          tasks: [
            {
              status: "inwork",
              importance: "high",
              text: "Learn vue.js"
            },
            {
              status: "done",
              importance: "ordinary",
              text: "Create some projects"
            },
          ]
        },
      ],
    };
  },
  components: { KanbanBoard }
}
</script>
