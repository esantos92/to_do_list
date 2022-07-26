<template>
  <div>
    <div 
      v-for="obj in toDos"
      :key="obj.id"
      class="todo-item"
    >
      {{ obj.title }}
    </div>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
    
  },
  data() {
    return {
      toDos: [
        {
        "userId": 1,
        "id": 1,
        "title": "Lorem ipsum",
        "completed": false
        },
        {
        "userId": 1,
        "id": 2,
        "title": "catacumba vazia",
        "completed": false
        },
        {
        "userId": 1,
        "id": 3,
        "title": "Paranaue",
        "completed": false
        },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.todo-item {
  background-color: #000;
  margin: 0 0 5px 0;
  padding: 3px 6px;
  color: #fff;
}
</style>
