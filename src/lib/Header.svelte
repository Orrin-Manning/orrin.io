<script lang="ts">
  export let showSignup: () => void;
  export let username = 'guest';
  export let path = '~';
</script>

<header class="flex justify-between items-baseline px-3 py-3">
  <h1 class="flex font-mono font-bold">
    <div>{'['}</div>
    <div>{`${username}@`}</div>
    <div>orrin.io</div>
    <pre>{` ${path}`}</pre>
    <div>{']$'}</div>
  </h1>
  <button
    on:click={showSignup}
    class="px-3 py-2 font-medium text-red-600 border-2 border-red-600 rounded-xl">Sign In</button
  >
</header>
