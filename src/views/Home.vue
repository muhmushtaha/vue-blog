<template>
  <div class="home">
    <PostsList />
  </div>
</template>

<script>
// @ is an alias to /src
import PostsList from '../components/postsList/index.vue';

export default {
  name: 'Home',
  components: {
    PostsList,
  },
};
</script>
