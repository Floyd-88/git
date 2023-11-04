<script setup>
import { defineProps, defineEmits } from 'vue'
defineProps({
    searchWord: {
        type: String,
        require: ""
    }
})
defineEmits(['update:searchWord', 'goSearch'])

</script>

<template>
  <aside>
    <ul>
      <li><a href="#">Ссылка 1</a></li>
      <li><a href="#">Ссылка 2</a></li>
      <li><a href="#">Ссылка 3</a></li>
      <li><a href="#">Ссылка 4</a></li>
      <li><a href="#">Ссылка 5</a></li>
      <li><a href="#">Ссылка 6</a></li>
      <li><a href="#">Ссылка 7</a></li>
    </ul>

    <div>
        <label for="search">Поиск на стрнице:</label> <br>
        <input id="search" 
        name="search" 
        type="text" 
        :value="searchWord" 
        @input="$emit('update:searchWord', $event.target.value)">
        <button @click="$emit('goSearch')">Поиск</button>
    </div>
  </aside>
</template>

<style scoped>
aside {
    display: grid;
    grid-template-rows: 1fr auto;
  flex: 1;
  padding: 5px;
  border: 1px solid gray;
  border-radius: 10px;
  background-color: gray;
}

li {
  padding: 5px 10px;
  list-style-type: none;
}

a {
  font-size: 17px;
  color: rgb(18, 17, 17);
  text-decoration: none;
}
a:hover {
  color: whitesmoke;
}
</style>
