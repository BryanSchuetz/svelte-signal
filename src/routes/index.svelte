<script>
  export const allposts = import.meta.glob('/src/lib/posts/*.md')
  export let attributes;
  export let html;
  let list = [];
  for (const path in allposts) {
    allposts[path]().then((mod) => {
      list.push({title: mod.attributes.title, path: path.replace("/src/lib/posts","blog").replace(".md","")});
      list = list;
    })
  }
</script>

<ul>
  {#each list as post, i}
    <li>
      <a href="{post.path}">{post.title}</a>
    </li>
  {/each}
</ul>
	

<style lang="scss">
	:root {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
</style>
