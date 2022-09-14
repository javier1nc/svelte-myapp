<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'
  export let name;
</script>

<main>
  <h1>Hello {name}</h1>
</main>

<style>
  h1{
    color: purple;
  }
</style>
