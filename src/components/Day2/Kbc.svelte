<script>
  import { each, select_options } from "svelte/internal";

  let pages = [
    {
      question: "who is prime ministor of india?",
      options: ["modi", "rahul gandhi", "amit shah", "yogi"],
      correct: 0,
      userOption: -1,
    },
    {
      question: "who is home ministor of india?",
      options: ["modi", "rahul gandhi", "amit shah", "yogi"],
      correct: 2,
      userOption: -1,
    },
    {
      question: "what is age of abhishrk gupta",
      options: [2, 34, 20, 18],
      correct: 3,
      userOption: -1,
    },
  ];
</script>

<h1>Kbc</h1>

{#each pages as page, i}
  <p>quention-{i + 1}</p>
  <p>{page.question}</p>

  {#each page.options as option, optionIndex}
    <button
      class={page.userOption === optionIndex ? "selected" : ""}
      on:click={() => {
        if (page.userOption === -1) {
          page.userOption = optionIndex;
        }
      }}>{option}</button
    >
  {/each}
  {#if page.userOption === -1}
    <p>please select the option</p>
  {:else if page.userOption === page.correct}
    <p>correct answer</p>
  {:else}
    <p>wrong answer</p>
  {/if}
{/each}

<style>
  .selected {
    border: 4px solid blue;
  }
</style>
