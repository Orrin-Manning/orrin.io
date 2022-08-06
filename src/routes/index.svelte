<script lang="ts">
  type socialButton = {
    icon: string;
    text: string;
    link: string;
    fgColor: string;
    bgColor: string;
  };

  let socialButtons: socialButton[] = [
    {
      icon: 'fa-github',
      text: 'Follow me on Github',
      link: 'https://github.com/Orrin-Manning',
      fgColor: 'text-white',
      bgColor: 'bg-neutral-900'
    },
    {
      icon: 'fa-linkedin-in',
      text: 'Connect on Linkedin',
      link: 'https://linkedin.com/in/orrin-manning-120509226',
      fgColor: 'text-white',
      bgColor: 'bg-blue-500'
    },
    {
      icon: 'fa-youtube',
      text: 'Subscribe to my channel',
      link: 'https://www.youtube.com/channel/UCnF65HkrWqwA3OWrJJ9O55w',
      fgColor: 'text-white',
      bgColor: 'bg-red-600'
    },
    {
      icon: 'fa-twitter',
      text: 'Follow me on Twitter',
      link: 'https://twitter.com/OrrinManning',
      fgColor: 'text-white',
      bgColor: 'bg-blue-400'
    }
  ];
</script>

<svelte:head>
  <script src="https://kit.fontawesome.com/46fb02e244.js" crossorigin="anonymous"></script>
</svelte:head>

<main class="flex flex-col items-center">
  <ul>
    {#each socialButtons as button, i}
      <li class="mb-4 last:mb-0">
        <a href={button.link} class="flex p-4 {button.fgColor} {button.bgColor} rounded-2xl">
          <span class="fa-brands {button.icon} mr-4 text-2xl" />
          <span class="flex-grow font-sans text-center">{button.text}</span>
        </a>
      </li>
    {/each}
  </ul>
</main>
