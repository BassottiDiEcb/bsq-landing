<script lang="ts">
	import Header from '../components/Header.svelte';

  export let title: string, image: string;
</script>

<div class="flex items-center justify-center h-44 p-8 bg-center bg-cover" style={`background-image: url(/${image}.jpg);`}>
  <Header />    
</div>

<div class="p-4 flex flex-col gap-y-8">
  <h1 class="font-bold text-3xl">{title}</h1>

  <slot />
</div>