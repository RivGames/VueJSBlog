<template>
  <div class="post" v-for="post in posts">
    <div><strong>Название:{{post.title}}</strong> Описание: {{post.body}}</div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.post {
  padding: 15px;
  border: 3px solid teal;
  margin-top: 15px;
}
</style>