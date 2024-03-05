<!--App.svelte file-->

<!--$: variableName -->

<script>
  let name = "Mustafa"

  let year = 2024

  $: greeting = "Welcome " + name + " and " + year + " will be your year!"
  
</script>

<input type="text" bind:value={name}>

<h1>Name: {name}</h1>

<h3>Year: {year}</h3>

<h2>{greeting}</h2>

<style>


</style>
