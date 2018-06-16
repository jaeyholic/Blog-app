<template>
  <div class="admin-new-post-page">
    <div class="new-post-form">
      <AdminPostForm />
    </div>
  </div>
</template>

<script>
  import AdminPostForm from '@/components/Admin/AdminPostForm'
 

  export default {
    components: {
      AdminPostForm
    }
  }
</script>

<style scoped>
.new-post-form {
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .new-post-form {
    width: 500px;
  }
}
</style>