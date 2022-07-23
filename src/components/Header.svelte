<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

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
</div>
