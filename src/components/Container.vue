<template>
  <div>
    <Post :postdata = "postdata[i]" v-for="(post,i) in postdata" :key="post"/>
  </div>

</template>

<script>
import Post from './Post.vue'
export default {
  name: 'container',
  components: {
    Post
  },
  props: {
    postdata: Array,
  }
}
</script>

<style>

</style>