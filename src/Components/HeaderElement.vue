<template>
      <header>
    <div class="logo"><a href="#">LOGO</a></div>
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Content</li>
      <li>Contacts</li>
    </ul>
  </header>
</template>

<style scoped>

header {
  display: flex;
  flex-direction: row;
  align-items: center;
  height: 100px;
  flex: 0 0 auto;
  background-color:slategrey
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
</style>