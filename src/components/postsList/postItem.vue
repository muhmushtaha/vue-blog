<template>
  <li class="posts-list-item">
    <div>
      <h2 class="post-title">{{ post.title }}</h2>
      <p class="post-content">{{ post.content }}</p>
    </div>
  </li>
</template>

<script>
export default {
  name: 'PostItem',
  props: {
    post: Object,
  },
};
</script>
<style lang="scss" scoped>
.posts-list-item {
  text-align: left;
  background-color: #fff;
  padding: 16px;
  border-radius: 4px;
  margin-bottom: 24px;
  box-shadow: 0px 0px 4px #e2e2e2;
  &:last-child {
    margin-bottom: 0;
  }
  .post-title {
    margin-bottom: 8px;
  }
}
</style>
