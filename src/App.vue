<template>
  <header>
    <NavBar />
  </header>
  <main>
    <Content />
  </main>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Content from './components/Content.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Content
  }
}
</script>

<style>

</style>
