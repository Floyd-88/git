<template>
  <main>
    <h1>Заголовок</h1>
    <div class="wrapper_main">
      <div class="content">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quia dolorum et cum debitis ab
        dignissimos, pariatur distinctio nesciunt eaque doloribus ullam inventore. Provident
        assumenda alias, cum quia at veritatis reprehenderit exercitationem eaque quam ullam,
        cupiditate fuga illum modi autem quas, dicta fugit magni molestias eveniet natus iusto
        repudiandae eos. Eveniet placeat itaque, incidunt sunt quis delectus autem fugit rem nam hic
        tenetur sint inventore magni, beatae excepturi reprehenderit totam mollitia officia
        quibusdam in neque labore magnam. Possimus deserunt fugiat consectetur nemo accusamus
        voluptas amet ipsa magni provident totam enim culpa quibusdam neque placeat odit, est non
        quidem, tempore quis perferendis.
      </div>
      <aside>
        <div>какое-то содержание в правой части содержимого страницы</div>
      </aside>
    </div>
  </main>
</template>

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
.wrapper_main {
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

aside {
    flex: 1;
    padding: 5px;
    border: 1px solid gray;
    border-radius: 10px;
    background-color:gray;
}
</style>
