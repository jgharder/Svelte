<script>
  export let name;
  export let image;
  export let music;
  export let hacker;
</script>

<tr>
  <td>
    {name}
  </td>
  <td >
    <img src={image} alt="This is me" />
  </td>

  <td >
    {music}
  </td>
  <td >
    {hacker}
  </td>
</tr>

<style>
 td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
