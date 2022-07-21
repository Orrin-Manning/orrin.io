<script lang="ts">
  export let username = 'guest';
  export let path = '~';
</script>

<div class="site-header">
  <h1>
    <code style=" display: flex; flex-wrap: false">
      <p class="logo-string">{'['}</p>
      {#if username}
        <p class="logo-string">{`${username}@`}</p>
      {/if}
      <p class="logo-string">orrin.io</p>
      {#if path}
        <p class="logo-string logo-path">{` ${path}`}</p>
      {/if}
      <p class="logo-string">{']$'}</p>
    </code>
  </h1>
</div>

<style>
  .site-header {
    display: flex;
    justify-content: left;
  }

  .logo-string {
    margin: 0;
  }

  .logo-path {
    white-space: pre;
  }
</style>
