<script lang="ts">
	export let href: string, text: string;
</script>

<a
	{href}
	class="underline-offset-8 hover:underline"
>
	{text}
</a>
