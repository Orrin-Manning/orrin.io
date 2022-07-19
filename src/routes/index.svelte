<script>
  let path = '';

  let user = {
    name: ''
  };
</script>

<div class="logo-container">
  <h1>
    <code style=" display: flex; flex-wrap: false">
      <p class="logo-string">{'['}</p>
      {#if user?.name}
        <p class="logo-string">{`${user?.name}@`}</p>
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
  .logo-container {
    display: flex;
    justify-content: center;
  }

  .logo-string {
    margin: 0;
  }

  .logo-path {
    white-space: pre;
  }
</style>
