<template>
  <main class="task-list" aria-label="Library tasks">
    <h2 class="task-list-title">Library Tasks</h2>
    <div class="task-items">
      <TaskItemComponent
        v-for="task in tasks"
        :key="task.id"
        :title="task.title"
        :description="task.description"
        :status="task.status"
      />
    </div>
  </main>
</template>

<script>
import TaskItemComponent from './task-item.component.vue'

export default {
  name: 'TaskListComponent',
  components: {
    TaskItemComponent
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: 'Return "The Great Gatsby"',
          description: 'Book due back to the library by Friday',
          status: 'Pending'
        },
        {
          id: 2,
          title: 'Review new book arrivals',
          description: 'Check and catalog 15 new books received today',
          status: 'In Progress'
        },
        {
          id: 3,
          title: 'Update author database',
          description: 'Add information for 3 new authors',
          status: 'Completed'
        }
      ]
    }
  }
}
</script>

<style scoped>
.task-list {
  flex: 1;
  padding: 2rem;
  background-color: #ffffff;
}

.task-list-title {
  margin: 0 0 1.5rem 0;
  font-size: 1.5rem;
  color: #2c3e50;
  font-weight: 600;
}

.task-items {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
</style>
