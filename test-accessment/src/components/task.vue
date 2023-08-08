<template>
<div id="app">
        <table class="todo-table">
            <thead>
                <tr>
                    <th>Todo Name</th>
                    <th>Progress Status</th>
                    <th>Actions</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(todo, index) in todos" :key="index">
                    <td>{{ todo.name }}</td>
                    <td>{{ todo.progress }}% Complete</td>
                    <td>
                        <button @click="editTodo(index)" class="edit-button">Edit</button>
                        <button @click="updateProgress(index)" class="update-button">Update</button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
    
</template>

<script>
export default {
  name: "task",
  data() {
    return {
      todos: [
        { name: "First Accessment", progress: 25 },
        { name: "Second Accessment", progress: 50 },
        { name: "Third Accessment", progress: 75 },
      ],
    };
  },
  methods: {
    editTodo(index) {
      console.log("Edit:", index);
    },
    updateProgress(index) {
      console.log("Update:", index);
    },
  },
};
</script>