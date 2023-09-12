<script lang="ts">
	import { Link } from "svelte-routing";

	export let image: string, title: string, href: string;
</script>

<article
	class="bg-cover h-64 bg-center flex flex-col gap-y-8 p-8 items-center justify-center bg-gray-400 bg-blend-multiply"
	style={`background-image: url(/${image}.jpg);`}
>
	<p class="text-2xl font-bold text-white">{title}</p>

	<Link
		class="p-2 border-2 border-white text-white font-bold uppercase hover:bg-white hover:text-slate-900"
		to={href}>Scopri di più</Link
	>
</article>
