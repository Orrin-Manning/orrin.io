<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

<header class="flex justify-between items-baseline px-3 py-3">
  <h1 class="flex font-mono font-bold">
    <div>{'['}</div>
    {#if username}
      <div>{`${username}@`}</div>
    {/if}
    <div>orrin.io</div>
    {#if path}
      <pre>{` ${path}`}</pre>
    {/if}
    <div>{']$'}</div>
  </h1>
  <button class="px-3 py-2 font-medium text-red-600 border-2 border-red-600 rounded-lg"
    >Sign In</button
  >
</header>
