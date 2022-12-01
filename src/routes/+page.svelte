<script>
  import Greet from "$lib/Greet.svelte";
</script>

<h1 class="text-center">Welcome to Tauri!</h1>

<div class="flex justify-center">
  <a href="https://vitejs.dev" target="_blank">
    <img
      src="/vite.svg"
      class="h-6rem p-1.5rem will-change-auto transition duration-750 hover:drop-shadow-[0_0px_2rem_#747bff]"
      alt="Vite Logo"
    />
  </a>
  <a href="https://tauri.app" target="_blank">
    <img
      src="/tauri.svg"
      class="h-6rem p-1.5rem will-change-auto transition duration-750 hover:drop-shadow-[0_0px_2rem_#24c8db]"
      alt="Tauri Logo"
    />
  </a>
  <a href="https://kit.svelte.dev" target="_blank">
    <img
      src="/svelte.svg"
      class="h-6rem p-1.5rem will-change-auto transition duration-750 hover:drop-shadow-[0_0px_2rem_#ff3e00]"
      alt="Svelte Logo"
    />
  </a>
</div>

<p class="text-center">
  Click on the Tauri, Vite, and Svelte logos to learn more.
</p>

<div class="flex justify-center">
  <Greet />
</div>
