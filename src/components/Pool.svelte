<script lang="ts">
  import Button from "smelte/src/components/Button";

  import { Sets } from "mtgsdk-ts";

  function handler() {
    Sets.all().on('data', (res) => console.log(res)).on('end', () => console.log('done'));
  }
</script>

<Button light on:click={handler}>Button</Button>
