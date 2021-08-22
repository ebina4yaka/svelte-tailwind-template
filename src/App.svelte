<script lang="ts">
  import Header from './Header.svelte'
  export let name: string
</script>

<header>
  <Header title="Svelte Tailwind Example" />
</header>
<main class="p-4">
  <h1 class="text-7xl text-center text-green-900 uppercase">Hello {name}!</h1>
  <p class="text-center p-4">
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
</main>

<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

  :global(body) {
    margin: 0;
    padding: 0;
  }
</style>
