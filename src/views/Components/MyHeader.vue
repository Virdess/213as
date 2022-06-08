<template>
  <nav class="navbar navbar-expand-lg bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <router-link to="/"><header-button>Главная</header-button></router-link>
        <header-button>Задачи</header-button>
        
      </ul>
    </div>
    <router-link to="/login"><header-button style="list-style-type: none;">Войти</header-button></router-link>
  </div>
</nav>
</template>

<script>
import HeaderButton from './UI/HeaderButton.vue'
export default {
  components: { HeaderButton },
name:'my-header',
}
</script>

<style>

</style>