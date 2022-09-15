<script lang="ts">
  import { onMount } from "svelte";
  import Name from "./lib/Name.svelte";

  let compName: Name;

  onMount(() => {
    // Type (mouse hover on `name`):   string
    console.log(compName.name_);
    // Type (mouse hover on `name`):   any
    console.log(compName.name);
  });
</script>

<Name bind:this={compName} />
