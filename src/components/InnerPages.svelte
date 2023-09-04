<script lang="ts">
	import Header from '../components/Header.svelte';

  export let title: string;
</script>

<div class="flex justify-center p-8">
  <Header />
  <h1 class="font-bold text-7xl">{title}</h1>
  <slot />
</div>