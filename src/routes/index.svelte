<script>
  import {html, attributes} from '$lib/content/2019-07-30-dry-the-rain.md'
</script>
	<h1 class="text-red-600 uppercase text-6xl font-thin leading-tight my-16 mx-auto max-w-xl">{attributes.title}</h1>
  <div>
    {@html html}
  </div>

	<p class="max-w-xs my-8 mx-auto leading-snug">Visit <a class="text-blue-600 underline" href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte apps.</p>

<style lang="scss">
	:root {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
</style>
