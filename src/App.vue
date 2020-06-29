<template>
  <div>
      <NavMenu></NavMenu>
      <h1>The Hunter Shall Surpass All Who Came Before Her</h1>
      <main>
      <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.pixabay.com%2Fphoto%2F2016%2F08%2F08%2F09%2F17%2Favatar-1577909_960_720.png&f=1&nofb=1" alt="">
      </main> 
  </div>
</template>

<script>
import NavMenu from './components/Landing/NavMenu.vue'

export default {
  name: 'App',
  components: {
    NavMenu
  }
}
</script>

<style>
@import './index.css'
</style>
