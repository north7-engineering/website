<script lang="ts">
  import "../app.css";
  import Navbar from "../lib/components/Navbar.svelte";
  import Footer from "../lib/components/Footer.svelte";
</script>

<Navbar />

<div class="mx-auto my-10 w-full max-w-screen-xl p-4 py-6 lg:py-8">
<slot />
</div>

<Footer />