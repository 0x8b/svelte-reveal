<script>
  import { onMount, tick } from 'svelte'
  import config from '$lib/config.js'
  import Presentation from './Presentation.svelte'
  import Reveal from 'reveal.js'

  onMount(async () => {
    await tick()

    const deck = new Reveal(config.reveal)

    deck.initialize()
  })
</script>

<div class="reveal">
  <div class="slides">
    <Presentation />
  </div>
</div>
