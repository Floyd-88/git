<template>
  <main>
    <h1>Заголовок</h1>
    <div class="main_wrapper">
      <div class="content">
        <div ref="article">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laudantium, temporibus?
        </div>
        <div ref="articleSearch">
        </div>
      </div>
      <AsideElement v-model:searchWord="searchWord" @goSearch="goSearch"/>
    </div>
  </main>
</template>
<script setup>
import AsideElement from '@/Components/AsideElement.vue'
import {ref, watch } from 'vue'

let searchWord = ref('')
let article = ref(null)
let articleSearch = ref(null)

function goSearch() {
      let reggie = new RegExp(searchWord.value, "ig");
      let found = article.value.innerHTML.search(reggie) !== -1;

    if(!found) {
      return article.value.innerHTML
    } else {
      article.value.style = 'display: none'
      return articleSearch.value.innerHTML = article.value.innerHTML.replace(reggie, '<b>' + searchWord.value + '</b>');

    } 
}

watch(searchWord, () => {
  articleSearch.value.innerHTML = ''
  article.value.style = 'display: block'
}) 

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
