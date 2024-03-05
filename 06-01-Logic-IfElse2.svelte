<!--App.svelte file-->

<script>

  let condition = false

  let toogleButton = () => {
    condition = !condition
  }
  
</script>

{#if !condition}

  <button on:click={toogleButton}>User Login</button>

  {:else} 
  <button on:click={toogleButton}>User Logout</button>

{/if}



<style>


</style>
