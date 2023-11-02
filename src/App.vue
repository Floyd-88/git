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
  <main></main>
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
  background-color: darkcyan;
}

footer {
  display: flex;
  flex-direction: row;
  height: 100px;
  flex: 0 0 auto;
  align-items: center;

  /* margin-top: auto; */
  background-color: lawngreen;
}

.copy{
  display: flex;
  flex-direction: column;
  flex: 1;
  align-items: center
}
</style>
