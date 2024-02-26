<!--App.svelte file-->

<script>

  let counter = 0

  let counterUp = () => {counter += 1}

  let counterDown = () => {counter -= 1}

</script>

<main>
  <h5>Mustafa Buyukdereli created this counter:)</h5>

  <button on:click={counterUp}>Counter ++</button>

  <input type="number" bind:value={counter}/>

  <button on:click={counterDown}>Counter --</button>
</main>

<style>

</style>
