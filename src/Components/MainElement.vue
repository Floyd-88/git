<template>
  <main>
    <h1>Заголовок</h1>
    <div class="main_wrapper">
      <div class="content">
        Lorem, ipsum dolor fgdkjgkl fgfkdj fgdajgioa fghioahgio
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

aside {
    flex: 1;
    padding: 5px;
    border: 1px solid gray;
    border-radius: 10px;
    background-color:gray;
}
</style>
