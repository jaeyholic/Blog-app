<template>
  <div>
    <section class="post-list">
      <PostPreview 
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
      previewText="This is my first Post"/>
      <PostPreview 
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
      previewText="This is my second Post"/>
    </section>
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';


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
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>