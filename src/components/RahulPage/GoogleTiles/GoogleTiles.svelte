<script>
  import Tile from "./Tile.svelte";

  const data = [
    {
      name: "(3) Feed",
    },
    {
      name: "https",
    },
    {
      name: "Udemy",
    },
    {
      name: "(1) WhatsApp",
    },
    {
      name: "GitHub",
    },
    {
      name: "Rahul Gupta",
    },
    {
      name: "Problems",
    },
    {
      name: "localhost",
    },
    {
      name: "Add shortcut",
    },
  ];
</script>

<div class="bg">
  <div class="items-container">
    {#each data as value}
      <Tile name={value.name} />
    {/each}
  </div>
</div>

<style>
  .bg {
    background-color: #6d41a1;
    height: 100%;
    min-height: 100vh;
  }
  .items-container {
    margin: auto;
    padding-top: 40vh;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    max-width: 560px;
  }
</style>
