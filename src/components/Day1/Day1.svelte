<script lang="ts">
  import Counter1 from "./Counter1.svelte";
  import Photo from "./Photo.svelte";
  import ViratKohli from "./ViratKohli.svelte";

  let name = "ahhi";
</script>

<main>
  <div>
    <h1>hello {name.toUpperCase()}</h1>

    <ViratKohli />
    <p>
      Lorem ipsum dolor, sit amet <strong> gorigr</strong> consectetur
      <em>higtrpg'h</em> adipisicing elit. Deserunt, iste.
    </p>
  </div>
  <div>
    <h2>hello raja</h2>
    <Photo />
    <Counter1 />
    <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
  </div>
</main>

<style>
  p {
    color: green;
    font-size: 30px;
  }
  h2 {
    color: aqua;
  }
</style>
