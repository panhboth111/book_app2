<template>
  <div>
    <div v-for="(post, index) in posts" :key="index">
      <h3>title : {{ post.title }}</h3>
      <h4>body: {{ post.index }}</h4>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data: () => ({
    posts: [],
  }),
  methods: {
    async getPosts() {
      const response = await axios.get(
        "https://jsonplaceholder.typicode.com/posts"
      );
      this.posts = response.data;
    },
  },
  created() {
    this.getPosts();
  },
};
</script>

<style></style>
