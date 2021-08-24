<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm.vue';
export default {
    components: {
        AdminPostForm
    },
    data(){
        return{
            loadedPost: {
                author: 'Peter',
                title: 'My awesome post',
                content: 'Super Amazing',
                thumbnailLink: 'https://cdn.pixabay.com/photo/2020/01/26/20/14/computer-4795762_1280.jpg',
            }
        }
    },
    layout: 'admin'
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