<script lang="ts">
  export let visible = true;
  export let hideSignup: () => void;
</script>

{#if visible}
  <div class="flex flex-col px-2 pt-16 pb-8 fixed inset-0 bg-black bg-opacity-75">
    <div class="flex flex-col p-8 h-full max-w-sm bg-white rounded-3xl">
      <button on:click={hideSignup} class="self-end w-8 h-8 relative">
        <div class="line rotate-45" />
        <div class="line -rotate-45" />
      </button>
    </div>
  </div>
{/if}

<style>
  .line {
    @apply w-full h-0.5 absolute inset-y-1/2 bg-black rounded -translate-y-1/2;
  }
</style>
