<script>
  export let name;
  let year = 2022;

  $: uppecaseName = name.toUpperCase();

  $: console.log(name);

  $: if (name=== "Javier"){
  console.log('It runs!')
    year = 2023;
  }


  function incrementYear(){
    year += 1;
  }
  function  changeName() {
    name = 'Javier';
  }

  function nameInput(event){
    const enteredValue = event.target.value;
    name = enteredValue;
  }

</script>

<main>
  <h1>Hello {uppecaseName}, {year}</h1>
  <button on:click="{incrementYear}">Change Yeard</button>
<!--  <button on:click="{changeName}">Change Name</button>-->
<!--  <input type="text" value="{name}" on:input="{nameInput}"> -->
  <input type="text" bind:value={name}>
</main>

<style>
  h1{
    color: orange;
  }
</style>
