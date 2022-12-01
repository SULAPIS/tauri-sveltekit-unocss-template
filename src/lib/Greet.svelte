<script lang="ts">
  import { invoke } from "@tauri-apps/api/tauri";

  let name = "";
  let greetMsg = "";

  async function greet() {
    // Learn more about Tauri commands at https://tauri.app/v1/guides/features/command
    greetMsg = await invoke("greet", { name });
  }
</script>

<div>
  <div class="flex justify-center">
    <input
      class=" rounded-lg border-1 border-transparent px-5 py-2.5 text-base font-medium font-inherit mr-1 color-#0f0f0f bg-#ffffff transition-[border] duration-250 shadow-lg shadow-grey-500/50 hover:border-#396cd8"
      placeholder="Enter a name..."
      bind:value={name}
    />
    <button
      class=" rounded-lg border-1 border-transparent px-5 py-2.5 text-base font-medium font-inherit mr-1 color-#0f0f0f bg-#ffffff transition-[border] duration-250 shadow-lg shadow-grey-500/50 hover:border-#396cd8"
      on:click={greet}
    >
      Greet
    </button>
  </div>
  <p>{greetMsg}</p>
</div>
