<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      previewText="lol"
      title="LOL"
      thumbnail="https://techcrunch.com/wp-content/uploads/2015/04/codecode.jpg?w=1390&crop=1"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      previewText="lol"
      title="LOL"
      thumbnail="https://techcrunch.com/wp-content/uploads/2015/04/codecode.jpg?w=1390&crop=1"
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      previewText="lol"
      title="LOL"
      thumbnail="https://techcrunch.com/wp-content/uploads/2015/04/codecode.jpg?w=1390&crop=1"
    />
  </section>
</template>

<script>
export default {
  props: {
    isAdmin: {
      type: Boolean,
      default: false
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
