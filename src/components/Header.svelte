<script lang="ts">
  import NavigationLink from './NavigationLink.svelte'
  import { scrolled } from '../stores/scrolled'
	import { Link } from 'svelte-routing';
</script>

<header
class="flex flex-col lg:flex-row gap-y-4 lg:gap-y-0 lg:w-2/3 w-11/12 mt-8 bg-opacity-20 rounded-lg justify-between items-center p-4 fixed top-0 transition-colors"
class:backdrop-blur={$scrolled}
class:bg-gray-700={$scrolled}
>
  <h1 class="font-bold text-2xl text-white">BSQ</h1>

  <nav class="flex lg:gap-x-12 text-sm text-md gap-x-6 text-center uppercase mt-5 lg:mt-0 text-white">
    <Link to="/" class="hover:underline underline-offset-8">Home</Link>

    {#if window.location.pathname === '/'}
      <NavigationLink href="#about_us" text="About us" />
      <NavigationLink href="#our_services" text="Our services" />
      <NavigationLink href="#learning" text="Learning" />
    {/if}
  </nav>
</header>