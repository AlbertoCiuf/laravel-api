<template>
<div class="wrapper">
    <Header />
    <div class="container">
    <PostContainer />
    </div>
</div>
</template>

<script>
import Header from '../components/partials/Header.vue';
import PostContainer from '../components/PostContainer.vue';

export default {
  name: 'App',
  components: {
    Header,
    PostContainer
  }
}
</script>

<style lang="scss">
.container {
  width: 70%;
  margin: 0 auto;
}
</style>