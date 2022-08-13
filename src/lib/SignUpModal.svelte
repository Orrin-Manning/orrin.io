<script lang="ts">
  export let visible = true;
  export let hideSignup: () => void;
</script>

{#if visible}
  <div class="flex flex-col px-2 pt-16 pb-8 fixed inset-0 bg-black bg-opacity-75">
    <div class="flex flex-col items-center p-8 max-w-sm bg-white rounded-3xl">
      <button on:click={hideSignup} class="self-end w-8 h-8 relative">
        <div class="line rotate-45" />
        <div class="line -rotate-45" />
      </button>
      <h1 class="mb-8 font-bold text-3xl">Sign Up</h1>
    </div>
  </div>
{/if}

<style>
  .line {
    @apply w-full h-0.5 absolute inset-y-1/2 bg-black rounded -translate-y-1/2;
  }
</style>
