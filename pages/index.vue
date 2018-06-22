<template>
 <div class="home-page">
   <section class="intro">
     <h1>Get the latest Tech news</h1>
   </section>

   <section class="featured-post">
      <PostList :posts="loadPosts"/>
    </section>
 </div>
</template>

<script>
import PostList from '@/components/Posts/PostList';


export default {
  components: {
    PostList
  },
  data() {
    return {
      loadPosts: [
        {
          id: '1',
          title: 'First Post',
          previewText: 'This is our first post',
          thumbnailLink: 'https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg'
        },
        {
          id: '2',
          title: 'Second Post',
          previewText: 'This is our second  post',
          thumbnailLink: 'https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg'
        }
      ]
    }
  }
}
</script>

<style>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('~assets/images/page-header.jpeg');
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1rem;
  text-align: center;
  color: #f4f9f4;
  background-color: rgb(32, 53, 65);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px #003545;
  box-sizing: border-box;
  border: 1px solid #003545;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-post {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
