<script>
  export let name;
  let year = 2022;

  $: uppecaseName = name.toUpperCase();
  $: name;

  function incrementYear(){
    year += 1;
  }
  function  changeName() {
    name = 'Javier';
  }
</script>

<main>
  <h1>Hello {uppecaseName}, {year}</h1>
  <button on:click="{incrementYear}">Change Yeard</button>
  <button on:click="{changeName}">Change Name</button>
</main>

<style>
  h1{
    color: orange;
  }
</style>
