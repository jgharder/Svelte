<script>
    import faker from '@faker-js/faker'
    import TableHead from './tableHead.svelte';
    import TableRow from './TableRow.svelte';

</script>


<table>
    {#each {length: 5} as _}
<TableHead/>
<TableRow 
name={faker.name.findName()}
image={faker.image.avatar()}
music={faker.music.genre()} 
hacker={faker.hacker.phrase()}
/>
{/each}

</table>


<style>
 table{
  border: 1px solid black;
  border-collapse: collapse;
}
</style>