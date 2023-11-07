<template>
  <main>
    <h1>Заголовок</h1>
    <div class="main_wrapper">
      <div class="content">
        <div ref="article" v-for="(text, index) in arrayText" :key="index">
          {{ text }}
        </div>
      </div>
      <AsideElement v-model:searchWord="searchWord" @goSearch="goSearch" />
    </div>
  </main>
</template>
<script setup>
import AsideElement from '@/Components/AsideElement.vue'
import { ref, defineProps } from 'vue'

// eslint-disable-next-line no-unused-vars
let props = defineProps({
  arrayText: {
    type: Array
  }
})

let searchWord = ref('')


</script>
<style scoped>
main {
  flex: 1 0 auto;
  padding: 0 20px;
  background-color: silver;
}
h1 {
  display: flex;
  justify-content: center;
  margin: 20px;
}
.main_wrapper {
  display: flex;
  flex-direction: row;
  height: 80%;
}

.content {
  flex: 3;
  margin-right: 10px;
  padding: 5px;
  border: 1px solid whitesmoke;
  border-radius: 10px;
  background-color: whitesmoke;
  font-size: 17px;
  line-height: 1.5rem;
}
</style>
