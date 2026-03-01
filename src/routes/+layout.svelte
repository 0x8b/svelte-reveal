<script>
  import './layout.css'
  import config from '$lib/config.js'
  import favicon from '$lib/assets/favicon.svg'

  let { children } = $props()
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
  <title>{config?.app?.name ?? 'Reveal.js with Svelte and Tailwind'}</title>
</svelte:head>

{@render children?.()}
