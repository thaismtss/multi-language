<template>
<div class="container">
  <h1 class="title">{{ $t('message') }}</h1>
  <div class="container-btns">
    <nuxt-link class="btn" :to="switchLocalePath('pt')">Português</nuxt-link>
    <nuxt-link class="btn" :to="switchLocalePath('en')">English</nuxt-link>
  </div>
</div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style scoped>
  .container {
    width: 100vw;
    height: 100vh;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
  }  
  .container-btns {
    display: flex;
  }
  .btn {
    text-decoration: none;
    background: rgb(44, 162, 220);
    color: white;
    padding: 1rem;
    font-size: 1.5rem;
    width: 120px;
    margin: 0.5rem;
    text-align: center;
  }
  .nuxt-link-exact-active {
    font-weight: bold;
    background: rgb(36, 139, 191);
    
}
</style>
