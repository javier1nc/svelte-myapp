<script>
  export let name;
  let year = 2022;

  function incrementYear(){
    year += 1;
  }
</script>

<main>
  <h1>Hello {name}, {year}</h1>
  <button on:click="{incrementYear}">Change Yeard</button>
</main>

<style>
  h1{
    color: orange;
  }
</style>
