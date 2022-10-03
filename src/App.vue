<template>
  <div id="app">

  </div>
</template>
<script>
import PostForm from '/@/components/PostForm.vue';
import PostList from '/components/PostList';
export default {
  data() {
    return {
      posts:[
        {id:1,title:'JavaScript',body:'lorem ipsum dolor sit amet'},
        {id:2,title:'JavaScript',body:'lorem ipsum dolor sit amet'},
        {id:3,title:'JavaScript',body:'lorem ipsum dolor sit amet'},
      ],
      title:'',
      body:'',
    }
  },
  methods: {
    createPost(){
      const newPost = {
        id:Date.now(),
        title:this.title,
        body:this.body,
      }
      this.posts.push(newPost);
      this.title = '';
      this.body = '';
    },
  }
}
</script>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app{
  padding:20px;
}
</style>