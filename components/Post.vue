<template>
  <nuxt-link :to="'/products/' + id">
    <div class="post">
      <p>{{ id }}.{{ title }}</p>
    </div>
  </nuxt-link>
</template>
<script>
export default {
  name: 'Post',
  props: ['id', 'title'],
}
</script>
<style>
.post {
  border-radius: 5px;
  background: whitesmoke;
  padding: 10px 15px;
  margin-bottom: 7px;
  color: #2d3436;
}
.post:hover {
  background: wheat;
  border: 1px solid blue;
}
a {
  text-decoration: none;
}
</style>