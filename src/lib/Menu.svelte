<script>
  import Logo from "./Logo.svelte";
  const navLinks = [
    { href:'/', label:'home' },
    { href:'/about', label:'about' },
    { href:'/projects',label:'projects' },
    { href:'/contact',label:'contact' }
  ]
</script>

<a href="/">
  <Logo />
</a>

{#each navLinks as {href, label}}
  <a {href} class="border-b-2 border-transparent hover:text-gray-800 transition-colors duration-300 transform dark:hover:text-gray-200 hover:border-blue-500 mx-1.5 sm:mx-6">{label}</a>
{/each}

<!-- <a href="/" class="text-gray-800 transition-colors duration-300 transform dark:text-gray-200 border-b-2 border-blue-500 mx-1.5 sm:mx-6">home</a> -->
