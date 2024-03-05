<!--App.svelte file-->

<script>

  import Employee from "./components/Employee.svelte";

  let employees = [
    {id: 1, name: "Mustafa Büyükdereli", department: "Future Innovations", wage: "$10000"},
    {id: 2, name: "Aygün Kaplan", department: "Finance Operations", wage: "$3000"},
    {id: 3, name: "John Nash", department: "RD", wage: "$8000"},
  ]

  const removeEmployee = () => {
    employees = employees.slice(1)
  }

</script>

{#each employees as e (e.id) }

  <Employee {...e}/>

  {:else}
  <h3>No employee remains!</h3>
  <!-- <Employee name={e.name} department={e.department} wage={e.wage}/> -->
    
{/each}

<button on:click={removeEmployee}>Remove Employee</button>


<style>


</style>
