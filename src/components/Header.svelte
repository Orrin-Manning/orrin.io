<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

<div class="container">
  <h1>
    <code style=" display: flex; flex-wrap: false">
      <div>{'['}</div>
      {#if username}
        <div>{`${username}@`}</div>
      {/if}
      <div>orrin.io</div>
      {#if path}
        <div class="path">{` ${path}`}</div>
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

  .path {
    white-space: pre;
  }
</style>
