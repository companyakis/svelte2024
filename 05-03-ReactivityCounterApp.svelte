<!--App.svelte file-->

<!--$: variableName -->

<script>

  let counter = 0

  $: info = counter

  const handleClick = () => {
    counter = counter * counter + 1
  }
  
</script>

<button on:click={handleClick}>Counter: {counter}</button>

<p>Counter info: {info}</p>

<style>


</style>
