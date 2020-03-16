<template>
  <div class="container">
    <div class="warning">
      Дорогие, жюри. В своем проекте мы использовали NLP ML, разработка заняла много времени, и бэк у нас практический не готов и фронт работает с текстом-рыбой. Но мы успешно протестировали модели и сохранили эмбеддинги в CSV, надеемся до вечера доделать проект и показать рабочий ресурс.
    </div>
    <div>
      <h1 class="title">Новостная лента</h1>
      <div class="posts">
        <Post v-for="post in posts" :key="post.id" :post="post" />
      </div>
    </div>
  </div>
</template>
<style scoped>
  .warning{
    margin: 20px 0;
    padding: 20px;
    background: orange;
    color: #fff;
    line-height: 1.5;
    font-size: 12px;
    text-transform: uppercase;
    font-weight: 600;
    border-radius: 10px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  }
</style>
<script>
import Logo from '~/components/Logo.vue'
import Post from '~/components/Post.vue'


export default {
  data(){
    return {
      posts: [
        {
          id: 1,
          title: "Коронавирус покоряет земли",
          content: "Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet ",
          created_at: "21 февраля 2019",
          url: "https://thesteppe.com/post/122"
        },
        {
          id: 1,
          title: "Коронавирус покоряет земли",
          content: "Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet ",
          created_at: "21 февраля 2019",
          url: "https://thesteppe.com/post/122"
        },
        {
          id: 1,
          title: "Коронавирус покоряет земли",
          content: "Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet ",
          created_at: "21 февраля 2019",
          url: "https://thesteppe.com/post/122"
        },
        {
          id: 1,
          title: "Коронавирус покоряет земли",
          content: "Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet ",
          created_at: "21 февраля 2019",
          url: "https://thesteppe.com/post/122"
        },
        {
          id: 1,
          title: "Коронавирус покоряет земли",
          content: "Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet Lorem ipsum dolor sit amet ",
          created_at: "21 февраля 2019",
          url: "https://thesteppe.com/post/122"
        }
      ]
    }
  },
  components: {
    Logo,
    Post
  }
}
</script>
