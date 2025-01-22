<template>
  <div>
    <h2>Input</h2>

    <div>
      <input name="input-text" type="text" class="mr-1" v-model="inputValue" />
      <button @click="addTodo" class="mr-1 add">+</button>
      <span>{{ inputValue }}</span>
    </div>

    <h2>ToDo</h2>
    <ul>
      <li v-for="(todo, index) in todos" :key="index">
        {{ todo }} <button @click="deleteTodo(index)" class="delete">x</button>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      inputValue: "",
      todos: [],
    };
  },
  methods: {
    addTodo() {
      this.todos.push(this.inputValue);
      this.inputValue = "";
    },
    deleteTodo(index) {
      this.todos.splice(index, 1);
    },
  },
};
</script>
<style>
ul {
  list-style-type: none;
  padding-left: 0;
  margin-top: 20px;
}
li {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f0edd7;
  margin: 8px 0;
  padding: 10px;
  border-radius: 5px;
  font-size: 16px;
  color: #333;
  transition: background-color 0.3s;
}

li:hover {
  background-color: #efcaca;
}

/* Кнопка удаления */
button.delete {
  background-color: #e74c3c;
  font-size: 14px;
  padding: 5px 10px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s;
}
button.add {
  background-color: #33dd2a;
  font-size: 14px;
  padding: 5px 10px;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s;
}

button.delete:hover {
  background-color: #c0392b;
}
</style>
