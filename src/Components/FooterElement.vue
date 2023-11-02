<template>
  <footer>
    <div class="logo"><a href="#">LOGO</a></div>
    <div class="copy">
      <div>Copyright Dio</div>
      <div>Designed By The Provided</div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  display: flex;
  flex-direction: row;
  height: 100px;
  flex: 0 0 auto;
  align-items: center;
  color:wheat;

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