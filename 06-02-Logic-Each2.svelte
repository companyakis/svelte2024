<!--App.svelte file-->

<script>

  import Employee from "./components/Employee.svelte";

  let employees = [
    {id: 1, name: "Mustafa Büyükdereli", department: "Future Innovations", wage: "$10000"},
    {id: 2, name: "Aygün Kaplan", department: "Finance Operations", wage: "$3000"},
    {id: 3, name: "John Nash", department: "RD", wage: "$8000"},
  ]


</script>

{#each employees as e (e.id) }

  <Employee {...e}/>

  <!-- <Employee name={e.name} department={e.department} wage={e.wage}/> -->

{/each}


<style>


</style>
