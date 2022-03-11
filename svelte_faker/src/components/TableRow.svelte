<script>
  export let name;
  export let image;
  export let music;
  export let hacker;
</script>

<tr>
  <td class="tablerow name">
    {name}
  </td>
  <td class="tablerow avatar">
    <img src={image} alt="This is me" />
  </td>

  <td class="tablerow music">
    {music}
  </td>
  <td class="tablerow hacker">
    {hacker}
  </td>
</tr>

<style>
 td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
