<template>
  <div>
    <h2>Products Page</h2>
    <Post
      v-for="post of posts"
      :key="post.id"
      :title="post.title"
      :id="post.id"
    />
  </div>
</template>

<script>
import axios from 'axios'
import Post from '../../components/Post.vue'
export default {
  layout: 'blog',
  components: {
    Post,
  },
  data() {
    return {
      posts: [],
    }
  },
  async created() {
    try {
      const res = await axios.get('https://jsonplaceholder.typicode.com/posts')
      this.posts = res.data
    } catch (error) {
      console.log(error)
    }
  },
}
</script>