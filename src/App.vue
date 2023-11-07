<script setup>
import FooterElement from '@/Components/FooterElement.vue';
import HeaderElement from '@/Components/HeaderElement.vue';
import MainElement from '@/Components/MainElement.vue';
import { ref } from 'vue';


let text = ref('')
let arrayText = ref([])
function addParagraph() {
arrayText.value.push(text.value)
text.value = ''

}
</script>

<template>
  <HeaderElement v-model="text" @addParagraph="addParagraph"/>
  
  <MainElement :arrayText="arrayText"/>
  
    <FooterElement />
    
</template>

<style scoped>
</style>
