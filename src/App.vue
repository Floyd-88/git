<script setup></script>

<template>
  <header>
    <div class="logo">LOGO</div>
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Content</li>
      <li>Contacts</li>
    </ul>
  </header>
  <main>
    <h1>Заголовок</h1>
    <div>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quia dolorum et cum debitis ab dignissimos, pariatur distinctio nesciunt eaque doloribus ullam inventore. Provident assumenda alias, cum quia at veritatis reprehenderit exercitationem eaque quam ullam, cupiditate fuga illum modi autem quas, dicta fugit magni molestias eveniet natus iusto repudiandae eos. Eveniet placeat itaque, incidunt sunt quis delectus autem fugit rem nam hic tenetur sint inventore magni, beatae excepturi reprehenderit totam mollitia officia quibusdam in neque labore magnam. Possimus deserunt fugiat consectetur nemo accusamus voluptas amet ipsa magni provident totam enim culpa quibusdam neque placeat odit, est non quidem, tempore quis perferendis.
    </div>
  </main>
  <footer>
    <div class="logo"><a href="#">LOGO</a></div>
    <div class="copy">
      <div>Copyright Dio</div>
      <div>Designed By The Provided</div>
    </div>
  </footer>
</template>

<style scoped>
header {
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 100px;
  flex: 0 0 auto;
  background-color: bisque;
}

.logo {
  flex: 1;
  text-align: center;
}

.logo>a {
  color:wheat
}
ul {
  flex: 1;
  display: flex;
  list-style-type: none;
  font-size: 20px;
  font-weight: 600;
}
ul > li {
  padding-right: 20px;
}

main {
  flex: 1 0 auto;
  background-color: silver
}
h1 {
  display: flex;
  justify-content: center;
  margin: 20px;
}

footer {
  display: flex;
  flex-direction: row;
  height: 100px;
  flex: 0 0 auto;
  align-items: center;
  color: wheat;
  /* margin-top: auto; */
  background-color: black;
}

.copy{
  display: flex;
  flex-direction: column;
  flex: 1;
  align-items: center
}
</style>
