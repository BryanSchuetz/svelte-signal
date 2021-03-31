<script context="module">
	export const prerender = true;
  export async function load({ page, fetch }) {
		const {html, attributes} = await import(`/src/lib/posts/${page.params.slug}.md`);
		return {
			props: {
				html: await html,
        attributes: await attributes
			}
		};
	}
</script>

<script>
  export let html;
  export let attributes;
</script>

<svelte:head>
	<title>{attributes.title}</title>
</svelte:head>

<div class="post">
  <h1>{attributes.title}</h1>
  <div>{@html html }</div>
</div>