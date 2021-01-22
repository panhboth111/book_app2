<template>
  <div class="home">
    <Book
      v-for="(book, index) in books"
      :key="index"
      :title="book.title"
      :description="book.description"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Book from "../components/Home/Book";
export default {
  name: "Home",
  components: {
    Book,
  },
  data: () => ({
    books: [
      {
        title: "Harry Potter",
        description: "this is a book",
      },
      {
        title: "Ream keeeee",
        description: "this is a bookkkkkk",
      },
      {
        title: "Ream keeeeeeeeeee",
        description: "this is a bookkkkkkkkkk",
      },
    ],
  }),
};
</script>
