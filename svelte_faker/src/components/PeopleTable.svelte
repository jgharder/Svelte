<script>
  import faker from "@faker-js/faker";
  import TableHead from "./tableHead.svelte";
  import TableRow from "./TableRow.svelte";

  const people = [];

  for (let i = 0; i < 1000; i++) {
    people.push({
      name: faker.name.findName(),
      image: faker.image.avatar(),
      music: faker.music.genre(),
      hacker: faker.hacker.phrase(),
    });
  }
</script>

<table>
  <TableHead col1="Name" col2="Image" col3="music" col4="Quote" />
  {#each people as person}
    <TableRow
      name={person.name}
      image={person.image}
      music={person.music}
      hacker={person.hacker}
    />
  {/each}
</table>

<style>
  table {
    border: 1px solid black;
    border-collapse: collapse;
  }
</style>
