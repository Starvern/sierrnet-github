<script lang="ts">
	import './layout.css';
	import '@fortawesome/fontawesome-free/css/all.min.css';
	import DisplaySection from '$lib/components/DisplaySection.svelte';
	import StarvernKnightPurple from '$lib/assets/StarvernKnightPurple.png';
	import SocialLink from '$lib/components/SocialLink.svelte';
	import { page } from '$app/state';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={StarvernKnightPurple} />
	<title>W.S. Portfolio</title>
</svelte:head>

<main class='font-regular font-[500] min-h-screen min-w-screen max-h-fit max-w-fit bg-[radial-gradient(circle,#00000025_1px,transparent_1px)]  bg-[size:1.25rem_1.25rem]'>
	<DisplaySection class='hidden md:block bg-white'>
		<div class='flex flex-row items-center px-[2rem] py-[1rem] gap-[5rem]'>
			<p>https://github.sierr.net{page.route.id}</p>
			<SocialLink link='/' label=home class='ml-auto'>
				Home
			</SocialLink>
			<SocialLink link='/design' label=design>
				Design
			</SocialLink>
		</div>
	</DisplaySection>
	{@render children()}

	<div class='mt-[5rem] h-[5rem] w-full bg-white flex flex-row items-center'>
    	<p class='mx-auto text-stone-500 text-[1rem]'>Developed & Designed by William</p>
	</div>
</main>