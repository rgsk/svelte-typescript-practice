<script>
  let count = 0;
</script>

<h1>Create a Flex Container</h1>

<div class="flex-container">
  <div>{count}</div>
  <div>2</div>
  <div>3</div>
</div>
<button
  on:click={() => {
    count += 1;
  }}>add</button
>
<p>
  A Flexible Layout must have a parent element with the <em>display</em>
  property set to <em>flex</em>.
</p>

<p>
  Direct child elements(s) of the flexible container automatically becomes
  flexible items.
</p>

<style>
  .flex-container {
    display: flex;
    background-color: DodgerBlue;
  }
</style>
