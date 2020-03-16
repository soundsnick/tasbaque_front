<template>
  <div>
    <Header />
    <nuxt />
  </div>
</template>
<script>
  import Header from '~/components/Header.vue'

  export default{
    components: {
      Header
    }
  }

</script>

<style>
:root{
  --color-main: #3F51B5;
}
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
.container{
  max-width: 600px;
  position: relative;
  margin: auto;
}
a{
  text-decoration: none;
  color: inherit;
}
.title{
  font-size: 22px;
  color: #4d4d4d;
  margin-top: 20px;
}
</style>
