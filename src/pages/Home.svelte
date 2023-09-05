<script lang="ts">
	import Box from '../components/Box.svelte';
	import Header from '../components/Header.svelte';
	import Icon from '@iconify/svelte';
	import { scrolled } from '../stores/scrolled'
</script>

<div
	class="h-screen flex justify-center bg-center bg-cover"
	style="background-image: url(/sea.jpg);"
>
	<Header />

	<div class="h-[calc(100%-96px)] flex flex-col justify-center items-center text-white">
		<div class="flex flex-col gap-y-8 items-center justify-center lg:p-0 px-2">
			<p class="text-7xl font-bold">BSQ</p>
			<hr class="border border-b-white w-full" />
			<p class="lg:text-xl">Nulla è perenne tranne il cambiamento</p>
		</div>

		<a href="#about_us" class="absolute bottom-8 text-white text-6xl">
			<Icon class="animate-bounce" icon="mdi:chevron-down" />
		</a>

		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<!-- svelte-ignore a11y-no-static-element-interactions -->
		<div
			on:click={() => document.body.scrollIntoView()}
			class="fixed bottom-8 right-8 text-white text-6xl backdrop-blur bg-gray-700 bg-opacity-20 rounded-lg"
			class:hidden={!$scrolled}
		>
			<Icon icon="mdi:chevron-up" />
		</div>
	</div>
</div>
<div class="flex justify-center" id="about_us">
	<div class="lg:p-32 px-4 py-8 w-full flex flex-col items-center gap-y-12">
		<p class="font-bold text-3xl">DOVE CUORE E TECNOLOGIA CORRONO INSIEME SIAMO PRESENTI</p>
		<p class="leading-loose">
			Alla base del nostro lavoro ci sono elementi chiave come armonia, rispetto e gioco di
			squadra. Pur essendo cresciuti nel corso degli anni, coltiviamo un approccio da "piccola
			azienda" che ci rende, inoltre, veri e propri partner per i nostri clienti anche grazie a
			una lunga esperienza su prodotti e processi aziendali complessi. In ognuna delle nostre
			soluzioni infatti c'è un pezzo di noi, un valore unico e personale che, spesso, assume una
			forma unica per tutti i nostri partner o per i nostri prodotti creati all'interno della
			factory.
		</p>
	</div>
</div>
<div class="flex justify-center bg-stone-100" id="our_services">
	<div class="w-full lg:py-32 lg:px-32 px-2 py-8 flex flex-col gap-y-12">
		<p class="font-bold text-3xl text-center">I NOSTRI SERVIZI</p>

		<div class="grid lg:grid-cols-3 grid-cols-1 gap-8">
			<Box href="/telecomunicazioni" title="Telecomunicazioni" image="telecomunicazioni" />

			<Box
				href="/cloud"
				title="Cloud - Data Center & Cyber Security"
				image="cloud"
			/>
 
			<Box href="/energia" title="Energia" image="energia" />
			<Box href="/laser" title="Laser Scanner" image="laser" />
			<Box href="/virtuale" title="Realtà Virtuale" image="virtuale" />
			<Box href="/droni" title="Droni" image="droni" />
		</div>
	</div>
</div>
<div class="flex justify-center bg-black" id="learning">
	<div class="w-full lg:py-32 lg:px-96 px-4 py-8 flex flex-col text-white gap-y-12">
		<p class="font-bold text-3xl text-center">FORMAZIONE E CRESCITA</p>

		In BSQ "essere giovani" è una virtù. In partnership con il CENTRO ELIS è stato avviato un
		piano di formazione finalizzato all'inserimento in azienda di neolaureati e neodiplomati in
		materie tecniche ed ingegneristiche da collocare negli ambiti ICT, Netw ork Deployment e
		Facility Management. Formazione retribuita fin dalla fase di training. Tutti gli allievi
		selezionati partecipano ad un percorso di formazione intensiva, diviso tra aula e luogo di
		lavoro, affiancati da professfionfisti BSQ, che già lavorano su progetti sfidanti presso
		alcuni dei nostri principali Clienti, con una percentuale di assunzione post academy superiore
		all'85%
	</div>
</div>
<div class="flex lg:px-96 lg:py-8 px-2 py-8 bg-zinc-900 border-t-zinc-800 border-t">
	<div class="flex gap-x-36 text-white">
		<div class="flex flex-col gap-y-8">
			<p class="font-bold">OUR ADDRESS</p>

			Via Della Scrofa 57, 000186 Roma<br />
			P.IVA 15363011006
		</div>

		<div class="flex flex-col gap-y-8">
			<p class="font-bold">FOLLOW US</p>

			<div class="flex flex-row text-2xl gap-x-4">
				<Icon icon="mdi:twitter" />
				<Icon icon="mdi:linkedin" />
			</div>
		</div>
	</div>
</div>