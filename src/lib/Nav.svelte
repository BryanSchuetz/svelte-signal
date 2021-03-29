<script>
  let current ='home';
</script>

<nav>
  <a 
  class="text-blue-400 hover:text-blue-600"
  class:active="{current === 'home'}" 
  on:click="{() => current = 'home'}"
  href="/">Home</a>
  <a 
  class="text-blue-400 hover:text-blue-600" 
  class:active="{current === 'about'}"
  on:click="{() => current = 'about'}"
  href="/about">About</a>
</nav>

<style lang="scss">
  $text-red-600: rgba(220, 38, 38,);
  .active{
    color: $text-red-600;
  }
</style>