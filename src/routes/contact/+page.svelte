<script lang="ts">
  import { onMount } from 'svelte';
  let pageTitle = 'Contact - North7 Engineering';
  onMount(() => {
    document.title = pageTitle;
  });
</script>

<h1 class="regular-font text-black uppercase dark:text-white">Contact</h1>

<dl class="mt-14 max-w-md text-gray-900 divide-y divide-gray-200 dark:text-white dark:divide-gray-700">
    <div class="flex flex-col pb-3">
        <dt class="regular-font mb-1 text-gray md:text-lg dark:text-grey">Email address</dt>
        <dd class="regular-font text-lg font-semibold dark:text-white">marcus@icloud.com</dd>
    </div>
    <div class="flex flex-col py-3">
        <dt class="regular-font mb-1 text-gray md:text-lg dark:text-grey">Home address</dt>
        <dd class="regular-font text-lg font-semibold dark:text-white">Ripvägen 3, 352 42, Växjö, Sweden</dd>
    </div>
    <div class="flex flex-col pt-3">
        <dt class="regular-font mb-1 text-gray md:text-lg dark:text-grey">Phone number</dt>
        <dd class="regular-font text-lg font-semibold dark:text-white">+46 70 252 07 93</dd>
    </div>
</dl>
