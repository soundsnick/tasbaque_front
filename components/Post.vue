<template>
  <div class="post">
    <span class="post__title">{{ post.title }}</span>
    <span class="post__published">{{ post.created_at }}</span>
    <p class="post__paragraph">{{ post.content }}</p>
    <span class="post__source">Источник: <a :href="post.url">{{ post.url }}</a></span>
  </div>
</template>
<style scoped>
  .post{
    margin: 15px 0;
    padding: 20px;
    border: 1px solid rgba(0,0,0,.05);
    background: #fff;
    box-shadow: 0 1px 3px rgba(0,0,0,.04);
  }
  .post__title{
    font-size: 20px;
    margin-bottom: 3px;
    display: block;
    font-weight: 700;
    text-transform: uppercase;
    color: black;
  }
  .post__published{
    margin-bottom: 15px;
    display: block;
    color: grey;
    font-size: 15px;
  }
  .post__paragraph{
    line-height: 1.3;
    font-size: 15px;
  }
  .post__source{
    display: block;
    margin-top: 10px;
    font-size: 13px;
    color: grey;
    text-align: right;
  }
  .post__source a{
    color: var(--color-main);
  }
</style>
<script>
  export default{
    props: ['post']
  }
</script>
