<template>
  <div class="card">
    <h1>Detalles de tu producto</h1>
    <h2>{{ post.title }}</h2>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  data() {
    return {
      post: {},
    }
  },
  async created() {
    const response = await axios.get(
      'https://jsonplaceholder.typicode.com/posts/' + this.$route.params.id
    )
    this.post = response.data
  },
}
</script>