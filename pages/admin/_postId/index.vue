<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
export default {
  layout: "admin",
  data() {
    return {
      loadedPost: {
        author: "bob",
        title: "bob",
        content: "bob",
        thumbnailLink: "lol"
      }
    };
  }
};
</script>
