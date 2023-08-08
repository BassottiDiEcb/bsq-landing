<script lang="ts">
	import Button from "./Button.svelte";

  export let image: string, title: string;
</script>

<article class="bg-cover h-64 bg-center flex flex-col gap-y-8 p-8 items-center justify-center bg-gray-400 bg-blend-multiply" style={`background-image: ${image};`}>
  <p class="text-2xl font-bold text-white">{title}</p>
  <Button text="Scopri di più" />
</article>