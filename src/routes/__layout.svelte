<script lang="ts">
  import '../app.css';
  import Header from '../lib/Header.svelte';
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Saira" rel="stylesheet" />
</svelte:head>

<div class="min-h-screen text-amber-200 bg-zinc-800">
  <Header />
  <slot />
</div>
