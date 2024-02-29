<!--App.svelte file-->

<!--props-->

<script>

  import Calculations from "./components/Calculations.svelte";

  let counter = 0

  const increment = () => { counter += 5 };

  const decrement = () => { counter -= 5 };

</script>

  <button on:click={increment}>Up</button>

  <Calculations {counter} />

  <button on:click={decrement}>Down</button>

<style>

</style>
