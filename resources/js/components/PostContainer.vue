<template>
  <div>
    <h2>Tutti i post</h2>
    <SinglePost 
      v-for="(post, index) in posts" :key="`p${index}`"
      :post="post"
    />
  </div>
</template>

<script>
import SinglePost from './SinglePost.vue'
export default {
  name: 'PostContainer',
  components: {
    SinglePost
  },
  data() {
    return {
      posts: null
    }
  },
  methods: {
    getApiPosts() {
      axios.get('http://127.0.0.1:8000/api/posts')
      .then(res => {
        this.posts = res.data;
      })
    }
  },
  mounted() {
    this.getApiPosts();
  }
}
</script>

<style lang="scss">
  h2 {
    margin: 30px 0;
  }
</style>