<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

<div class="flex justify-start">
  <h1>
    <code>
      <div>{'['}</div>
      {#if username}
        <div>{`${username}@`}</div>
      {/if}
      <div>orrin.io</div>
      {#if path}
        <div class="whitespace-pre">{` ${path}`}</div>
      {/if}
      <div>{']$'}</div>
    </code>
  </h1>
</div>
