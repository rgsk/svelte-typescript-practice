<script lang="ts">
  let count: number = 0;
  $: doubled = count * 2;
  const increment = () => {
    count += 1;
  };
  $: {
    console.log(doubled);
  }
  $: if (count >= 10) {
    alert("count is dangerously high!");
    count = 9;
  }
</script>

<button on:click={increment}>
  <span class="text-red-500">count is {count}</span>
  <span class="text-green-500">doubled is {doubled}</span>
</button>
