<script lang="ts">
  import { onMount } from 'svelte';
  let pageTitle = 'North7 Engineering';
  onMount(() => {
    document.title = pageTitle;
  });
</script>