<template>
  <div>
    <h3>Title: {{ title }}</h3>
    <h4>Description:{{ description }}</h4>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String,
  },
};
</script>

<style></style>
