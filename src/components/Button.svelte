<script lang="ts">
	export let text: string,
		color: string = 'text-white',
		background: string = 'bg-transparent',
		border: string = 'border-white';
</script>

<!-- <button
	class={`text-uppercase px-4 py-2 border-2 ${color} ${background} ${border} hover:opacity-80 transition-all w-48`}
>
	{text}
</button> -->

<button
	class="uppercase px-4 py-2 border-2 text-white border-white bg-transparent hover:bg-white hover:text-black transition-all font-bold w-48"
>
	{text}
</button>