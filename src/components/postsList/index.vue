<template>
  <div class="posts-list-container">
    <ul class="posts-list">
      <PostItem v-for="post in postsList" :post="post" :key="post.id" />
    </ul>
  </div>
</template>

<script>
import postsListData from '../../constants/fakePostsData';
import PostItem from './postItem.vue';

export default {
  name: 'PostsList',
  components: {
    PostItem,
  },
  data() {
    return {
      postsList: postsListData,
    };
  },
};
</script>
<style lang="scss" scoped>
.posts-list {
  list-style-type: none;
}
</style>
