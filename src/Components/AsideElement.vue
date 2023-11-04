<script>
const documents = [
  {
    content: 'Ты был мне как брат! Я любил тебя!',
    author: 'Obi-Wan Kenobi',
    date: '2017-01-17 07:13:07'
  },
  {
    content: 'База повстанцев находится на Дантуине.',
    author: 'Leia Organa',
    date: '2019-11-27 21:33:56'
  },
  {
    content:
      'Страх открывает доступ к темной стороне! Страх рождает гнев, гнев рождает ненависть, ненависть — залог страданий.',
    author: 'Leia Organa',
    date: '1999-02-19 16:56:11'
  }
]

function getDocuments(documents) {
  let res = documents.reduce(
    (acc, item) => {
      acc.content += item.content
      acc.author.add(item.author)
      if (new Date(item.date).getTime() > new Date(acc.date).getTime()) {
        acc.date = item.date
      }
      return acc
    },
    {
      content: '',
      author: new Set(),
      date: null
    }
  )
  res.author = Array.from(res.author)
  return res
}
console.log(getDocuments(documents))
</script>

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

    <div>
        <label for="search">Поиск на стрнице:</label> <br>
        <input id="search" name="search" type="text">
    </div>
  </aside>
</template>

<style scoped>
aside {
    display: grid;
    grid-template-rows: 1fr auto;
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

a {
  font-size: 17px;
  color: rgb(18, 17, 17);
  text-decoration: none;
}
a:hover {
  color: whitesmoke;
}
</style>
