<script lang="ts">
  let showMenu: boolean = false;

  function toggleNavbar(): void {
    showMenu = !showMenu;
  }
</script>

<div class="border-gray-200 dark:bg-gray-900">
  <div>
    <nav class="container px-6 py-8 mx-auto md:flex md:justify-between md:items-center">
      <div class="flex items-center justify-between">
        <a href="https://flowbite.com/" class="flex items-center">
          <img src="https://flowbite.com/docs/images/logo.svg" class="h-8 mr-3" alt="Flowbite Logo" />
          <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">North7</span>
        </a>
        <!-- Mobile menu button -->
        <div on:click={toggleNavbar} class="flex md:hidden">
          <button
            type="button"
            class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                 stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <div
        class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0 {showMenu
          ? 'flex'
          : 'hidden'}"
      >
        <a class="text-gray-800 hover:text-blue-400" href="/home">Home</a>
        <a class="text-gray-800 hover:text-blue-400" href="/blog">Services</a>
        <a class="text-gray-800 hover:text-blue-400" href="/contact">Contact</a>
        <a class="text-gray-800 hover:text-blue-400" href="/about">About</a>
      </div>
    </nav>
  </div>
</div>