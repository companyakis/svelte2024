<!--App.svelte file-->

<!--props and default value-->

<script>
  import Calculations from "./components/Calculations.svelte";

  let counter = 0;

  const increment = () => {
    counter += 5;
  };

  const decrement = () => {
    counter -= 5;
  };
</script>

<button on:click={increment}>Up</button>

<Calculations {counter} />

<Calculations /> <!--default value-->

<button on:click={decrement}>Down</button>

<style>
</style>
