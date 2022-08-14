<script lang="ts">
  import '../app.css';
  import SignUpModal from '../lib/SignUpModal.svelte';
  import Header from '../lib/Header.svelte';

  let isSignup = false;

  const showSignup = () => {
    isSignup = true;
  };
  const hideSignup = () => {
    isSignup = false;
  };
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
  <link href="https://fonts.googleapis.com/css2?family=Raleway" rel="stylesheet" />
</svelte:head>

<SignUpModal visible={isSignup} {hideSignup} />
<div class="min-h-screen text-amber-200 bg-zinc-800">
  <Header {showSignup} />
  <slot />
</div>
