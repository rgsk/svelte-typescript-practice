<script>
  let n = 6;
  let multipliers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  //   let names = ["rahul", "mehak"];
</script>

<h1>Table</h1>

<input type="number" bind:value={n} />

<!-- <p>{n} * 1 = {n * 1}</p>
<p>{n} * 2 = {n * 2}</p>
<p>{n} * 3 = {n * 3}</p>
<p>{n} * 4 = {n * 4}</p>
<p>{n} * 5 = {n * 5}</p>
<p>{n} * 6 = {n * 6}</p>
<p>{n} * 7 = {n * 7}</p> -->

{#each multipliers as m}
  <p>{n} * {m} = {n * m}</p>
{/each}
