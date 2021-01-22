<template>
  <div id="app">
    <button><router-link to="/">Home</router-link></button><br />
    <button><router-link to="/about">about</router-link></button><br />
    <button><router-link to="/settings">settings</router-link></button><br />
    <router-view />
  </div>
</template>

<script>
export default {
  components: {},
  data: () => ({}),
  methods: {},
};
</script>
<style></style>
