<script setup>
import { defineProps, defineEmits } from 'vue'

defineProps({
  modelValue: {
    type: String
  }
}) 
let emit = defineEmits(['update:modelValue', 'addParagraph'])

function addParagraph() {
  emit('addParagraph')
}
</script>

<template>
  <header>
    <div class="logo"><a href="#">LOGO</a></div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Content</a></li>
      <li><a href="#">Contacts</a></li>
    </ul>

    <div class="addText">
      <input 
        placeholder="добавить новый абзац" 
        type="text" 
        :value="modelValue"
        @input="$emit('update:modelValue', $event.target.value)"
      />
      <button @click="addParagraph()">добавить</button>
    </div>
  </header>
</template>

<style scoped>
header {
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 100px;
  flex: 0 0 auto;
  background-color: slategrey;
}

ul {
  flex: 1;
  display: flex;
  list-style-type: none;
  font-size: 20px;
  font-weight: 600;
}
ul > li {
  margin-right: 20px;
  color: black;
}

ul > li > a {
  color: black;
  text-decoration: none;
}

a:hover {
  color: rgb(78, 44, 179);
}

.addText {
  margin-right: 20px;
}
</style>
