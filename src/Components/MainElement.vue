<template>
  <main>
    <h1>Заголовок</h1>
    <div class="main_wrapper">
      <div class="content">
        <div>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laudantium, temporibus?</div>
      </div>
      <AsideElement/>
    </div>
  </main>
</template>
<script setup>
import AsideElement from '@/Components/AsideElement.vue';


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
