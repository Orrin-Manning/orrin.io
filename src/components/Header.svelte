<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

<div class="container">
  <h1>
    <code style=" display: flex">
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

<style>
  .container {
    display: flex;
    justify-content: left;
  }
</style>
