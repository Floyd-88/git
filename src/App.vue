<script setup>
import FooterElement from '@/Components/FooterElement.vue';
import HeaderElement from '@/Components/HeaderElement.vue';

</script>

<template>
  <HeaderElement/>
  
  <main>
    <h1>Заголовок</h1>
    <div>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quia dolorum et cum debitis ab dignissimos, pariatur distinctio nesciunt eaque doloribus ullam inventore. Provident assumenda alias, cum quia at veritatis reprehenderit exercitationem eaque quam ullam, cupiditate fuga illum modi autem quas, dicta fugit magni molestias eveniet natus iusto repudiandae eos. Eveniet placeat itaque, incidunt sunt quis delectus autem fugit rem nam hic tenetur sint inventore magni, beatae excepturi reprehenderit totam mollitia officia quibusdam in neque labore magnam. Possimus deserunt fugiat consectetur nemo accusamus voluptas amet ipsa magni provident totam enim culpa quibusdam neque placeat odit, est non quidem, tempore quis perferendis.
    </div>
  </main>
  
    <FooterElement/>
    
</template>

<style scoped>
main {
  flex: 1 0 auto;
  background-color: silver
}
h1 {
  display: flex;
  justify-content: center;
  margin: 20px;
}

</style>
