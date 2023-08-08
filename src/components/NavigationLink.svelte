<script lang="ts">
	export let href: string, text: string;

	let underline = false;

	function handleClick() {
		const words = window.location.href.split('#');
		underline = words[1] == href;
	}
</script>

<a
	href={`#${href}`}
	on:click={handleClick}
	class="text-white underline-offset-8 hover:underline transition-all"
	class:underline
>
	{text}
</a>
