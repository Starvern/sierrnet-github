<script>
    import Navbar from '$lib/Navbar.svelte';
</script>

<main class='touch-manipulation overscroll-none overflow-auto bg-[#0a090c] w-screen pb-[2rem] max-h-full min-h-screen text-slate-200 font-mono flex flex-col gap-10'>
    <Navbar />
    <div class='mt-[5rem] md:mt-0'></div>
    <div class='touch-pan-y overscroll-none overflow-auto flex flex-col gap-5 md:gap-10 px-[1rem]'>
        <slot></slot>
    </div>
</main>