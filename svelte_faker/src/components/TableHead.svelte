<script>
  export let col1;
  export let col2;
  export let col3;
  export let col4;
</script>

<tr>  
  <th class="tablehead">
{col1}  </th>
  <th class="tablehead">
    {col2}
  </th>
  <th class="tablehead">
{col3}  </th>
  <th class="tablehead">
{col4}
  </th>
</tr>

<style>
  th{
  border: 1px solid black;
  border-collapse: collapse;
}
</style>