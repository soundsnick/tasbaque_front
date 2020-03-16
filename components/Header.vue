<template>
  <header class="header">
    <div class="container">
      <a class="logo">
        <span class="logo-text">Tasbaque</span>
      </a>
      <nav class="navigation">
        <a href="/" class="navigation__item">Лента</a>
        <a href="#" class="navigation__item">О проекте</a>
      </nav>
    </div>
  </header>
</template>
<style scoped>
  .header{
    background: #fff;
    border-bottom: 1px solid rgba(0,0,0,.04);
    padding: 20px 0;
    box-shadow: 0 1px 6px rgba(0,0,0,0.02);
  }
  .header .container{
    display: flex;
    justify-content: space-between;
  }
  .navigation__item{
    color: rgba(0,0,0,.6);
    padding: 0 10px;
    font-size: 14px;
    transition: color 0.2s;
  }
  .navigation__item:hover{
    color: var(--color-main);
  }
  .logo-text{
    text-transform: uppercase;
    font-weight: bolder;
    font-size: 19px;
    color: var(--color-main);
  }
</style>
