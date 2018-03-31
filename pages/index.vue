<template>
  <section class="container" id="post">
    <PostPreview
        v-for="post in posts"
        :key="post.id"
        :title="post.title"
        :excerpt="post.previewText"
        :thumbnailImage="post.thumbnailUrl"
        :id="post.id"
    >

    </PostPreview>
  </section>
</template>

<script>
import PostPreview from '../components/Blog/PostPreview'
  export default {
      components: {
          PostPreview
      },
      data(){
          return{
              posts:[
                  {
                      title:'A New Beginnig',
                      previewText:'This will be awesome,do not miss it!',
                      thumbnailUrl:'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2921719521,4265788220&fm=200&gp=0.jpg',
                      id:'a-new-beginning'
                  },
                   {
                      title:'A Second Beginnig',
                      previewText:'This will be awesome,do not miss it!',
                      thumbnailUrl:'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=2921719521,4265788220&fm=200&gp=0.jpg',
                      id:'a-second-beginning'
                  }
              ]
          }
      }
  }

</script>

<style scoped>

#post{
    padding-top:2rem;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
@media (min-width:35rem){
    #post{
        flex-direction: row;
    }
}
</style>
