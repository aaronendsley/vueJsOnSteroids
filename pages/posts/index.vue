<template>
  <div class="posts-page">
    <PostList :posts="loadedPosts" />
  </div>
</template>

<script>
export default {
  asyncData(context, callback) {
    setTimeout(() => {
      callback(null, {
        loadedPosts: [
          {
            id: "1",
            title: "first Post",
            previewText: "lol",
            thumbnail:
              "https://storage.googleapis.com/afs-prod/media/afs:Medium:5511630073/1900.png"
          },
          {
            id: "2",
            title: "second Post",
            previewText: "lol2",
            thumbnail:
              "https://storage.googleapis.com/afs-prod/media/afs:Medium:5511630073/1900.png"
          }
        ]
      });
    }, 1500);
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
