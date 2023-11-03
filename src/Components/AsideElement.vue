<template>
  <aside>
    <ul>
        <li><a href="#">Ссылка 1</a></li>
        <li><a href="#">Ссылка 2</a></li>
        <li><a href="#">Ссылка 3</a></li>
        <li><a href="#">Ссылка 4</a></li>
        <li><a href="#">Ссылка 5</a></li>
        <li><a href="#">Ссылка 6</a></li>
        <li><a href="#">Ссылка 7</a></li>


    </ul>
  </aside>
</template>

<style scoped>
aside {
  flex: 1;
  padding: 5px;
  border: 1px solid gray;
  border-radius: 10px;
  background-color: gray;
}

li {
    padding: 5px 10px;
    list-style-type: none;
}

a{
  font-size: 17px;
  color:rgb(18, 17, 17);
  text-decoration: none;
}
a:hover {
    color: whitesmoke;
}
</style>
