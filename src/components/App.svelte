<script>
  import router from 'page'
  import Home from './Home.svelte'
  import About from './About.svelte'

  let page

  router('/', () => page = Home)
  router('/about', () => page = About)

  router.start()
</script>
<svelte:component this={page}/>

<style>
</style>

