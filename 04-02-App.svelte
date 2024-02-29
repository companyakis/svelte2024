<!--App.svelte file-->

<!--spread props-->

<script>
  import Employee from "./components/Employee.svelte";

  const employeeInfo1 = {
    name: "Aygün Göğebakan",
    title: "CFO",
    about: "Finance expert over 10 years"
  }

  const employeeInfo2 = {
    name: "Kültigin Göktürk",
    title: "CEO",
    about: "Management expert over 25 years"
  }
</script>

<Employee {...employeeInfo1} />

<Employee {...employeeInfo2}/>

<style>
</style>
