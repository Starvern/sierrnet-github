<script lang="ts">
	import './layout.css';
	import '@fortawesome/fontawesome-free/css/all.min.css';
	import DisplaySection from '$lib/components/DisplaySection.svelte';
	import StarvernKnightPurple from '$lib/assets/StarvernKnightPurple.png';
	import { page } from '$app/state';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={StarvernKnightPurple} />
	<title>William Sierra | Avionics</title>
</svelte:head>

<main class='font-regular font-medium min-h-screen min-w-screen max-h-fit max-w-fit m-0 p-0'>
	<DisplaySection dark={false} class='border-b-2'>
		<div class='flex flex-row items-center px-8 py-4 gap-20'>
			<p class='hidden md:block'>https://sierr.net{page.route.id}</p>
		</div>
	</DisplaySection>

	{@render children()}

	<DisplaySection dark={true} class='text-center py-10 m-0'>
		<a href="https://github.com/Starvern/sierrnet-github">Developed & Designed by William</a>
	</DisplaySection>
</main>