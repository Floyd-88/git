<script setup>
import FooterElement from '@/Components/FooterElement.vue';
import HeaderElement from '@/Components/HeaderElement.vue';
import MainElement from '@/Components/MainElement.vue';
import { ref, computed } from 'vue';


let text = ref('')
let arrayText = ref([])
function addParagraph() {
arrayText.value.push(text.value)
text.value = ''

}

const upperCaseLetter = computed(() => {
  return arrayText.value.map((elem) => {
    return elem.slice(0, 1).toUpperCase() + elem.slice(1)
  })
})

</script>

<template>
  <HeaderElement v-model="text" @addParagraph="addParagraph"/>
  
  <MainElement :arrayText="upperCaseLetter"/>
  
    <FooterElement />
    
</template>

<style scoped>
</style>
