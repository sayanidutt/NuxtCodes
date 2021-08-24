<template>
    <section class="post-lists">
      <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://cdn.pixabay.com/photo/2020/01/26/20/14/computer-4795762_1280.jpg"
      title="Hello there"
      previewText="This is my first post" />
      <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://cdn.pixabay.com/photo/2020/01/26/20/14/computer-4795762_1280.jpg"
      title="Hello there the second time"
      previewText="This is my second post" />
      <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://cdn.pixabay.com/photo/2020/01/26/20/14/computer-4795762_1280.jpg"
      title="Hello there the third time"
      previewText="This is my third post" />
    </section>
</template>

<script>
import PostPreview from './PostPreview.vue';
export default {
    components: {
        PostPreview
    },
    props: {
      isAdmin: {
        type: Boolean,
        default: false
      }
    }
}
</script>

<style scoped>
.post-lists {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>