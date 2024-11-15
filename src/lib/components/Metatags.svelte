<script lang="ts">
  export let title = 'William Jojarth';
  export let description = "I'm William. I tell stories, and I'd love to tell yours.";
  export let image = '/favicon.ico';
</script>

<svelte:head>
	<title>{title}</title>
  <meta name="description" content={description}/>

  <meta property="og:title" content={title} />
  <meta property="og:description" content={description} />
  <meta property="og:image" content={image} />

  <link rel="icon" href="/favicon.ico" type="image/x-icon"/>
</svelte:head>