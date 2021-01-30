<script lang="ts">
  import "smelte/src/tailwind.css";
  import Pool from './components/Pool.svelte';
  // import Button from "smelte/src/components/Button";

  // import { allSets } from 'scryfall';

  // function handler() {
  //   allSets().then(res => console.log(res));
  // }
</script>

<style>
  main {
    background-color: var(--color-primary-50);
  }

  .area {
    border-radius: 5px;
    margin: 0.5rem 1rem;
    padding: 0.5rem;
    background-color: #eee;
  }

  .preview,
  .stats {
    width: 25%;
  }

  .pool,
  .deck {
    height: 50%;
  }
</style>

<main class="h-full flex bg-purple-300">
  <div class="area preview"></div>
  <div class="flex flex-col w-1/2">
    <div class="area pool">
      <Pool></Pool>
    </div>
    <div class="area deck"></div>
  </div>
  <div class="area stats"></div>
</main>
