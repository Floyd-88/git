<script setup>
</script>

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
    <footer></footer>
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
ul{
  flex: 1;
  display: flex;
  list-style-type: none;
  font-size: 20px;
  font-weight: 600;
  
}
ul>li {
  padding-right: 20px;
}

main {
  flex: 1 0 auto;
  background-color: darkcyan;
}

footer {
  height: 100px;
  flex: 0 0 auto;

  /* margin-top: auto; */
  background-color: slategray;
}

</style>
