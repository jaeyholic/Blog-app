<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPosts"/>
    </section>
  </div>
</template>

<script>
  import AdminPostForm from '@/components/Admin/AdminPostForm'

  export default {
    layout: 'admin',
    components: {
      AdminPostForm
    },
    data(){
      return {
        loadedPosts: {
        author: 'Jeff',
        title: 'My Awesome Title',
        content: 'Super amazing, thanks for that',
        thumbnailLink: 'https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg'
        }
      }
    }
  }
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>