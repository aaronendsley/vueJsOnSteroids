<template>
  <section class="post-list">
    <PostPreview
      v-for="post in posts"
      v-bind:key="post.key"
      :id="post.id"
      :is-admin="isAdmin"
      :previewText="post.previewText"
      :title="post.title"
      :thumbnail="post.thumbnail"
    />
  </section>
</template>

<script>
export default {
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    },
    posts: {
      type: Array,
      required: true
    }
  }
};
</script>
<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
