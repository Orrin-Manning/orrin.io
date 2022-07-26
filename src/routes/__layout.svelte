<script lang="ts">
  import '../app.css';
  import Header from '../components/Header.svelte';
</script>

<div class="min-h-screen text-amber-200 bg-zinc-800">
  <Header />
  <slot />
</div>
