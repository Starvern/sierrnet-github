<script>
    import { page } from '$app/state';
    import NavbarLink from '$lib/NavbarLink.svelte';

    let expanded = false;
    let navbarClass = "h-[5rem] delay-[0.5s]";
    let itemClass = "opacity-0 collapse";

    const expand = () => {
        expanded = !expanded;
        navbarClass = expanded ? 'h-[21.5rem]' : 'h-[5rem] delay-[0.5s]';
        itemClass = expanded ? 'opacity-100 delay-[0.5s]' : 'opacity-0';
    }

</script>

<div class='hidden bg-[#131116] relative w-full md:h-[5rem] md:flex md:flex-row md:p-[1rem] md:font-bold md:text-[1.5rem]'>
    <NavbarLink route='/' display='Home' />
    <NavbarLink route='/contact' display='Contact' />
    <NavbarLink route='https://github.com/Starvern' display='Github' />
    <NavbarLink route='/projects' display='Projects' />
    <NavbarLink route='/resume' display='Resume' />
</div>

<div class='fixed w-screen'>
    <div class='md:hidden bg-[#131116] mb-[10rem] w-full max-h-fit overflow-hidden flex flex-col p-[1rem] text-[1.5rem] ease-in-out transition-[height] duration-[1s] {navbarClass}'>
        <button on:click={expand} class='z-50 h-fit p-2 hover:bg-[#1b1821] active:bg-[#1b1821]'>☰</button>
    
        <inline class='flex flex-col {itemClass} transition-[opacity] ease-in-out duration-[0.25s]'>
            <NavbarLink route='/' display='Home' />
        </inline>
        <inline class='flex flex-col {itemClass} transition-[opacity] ease-in-out duration-[0.5s]'>
            <NavbarLink route='/contact' display='Contact' />
        </inline>
        <inline class='flex flex-col {itemClass} transition-[opacity] ease-in-out duration-[0.75s]'>
            <NavbarLink route='https://github.com/Starvern' display='Github' />
        </inline>
        <inline class='flex flex-col {itemClass} transition-[opacity] ease-in-out duration-[1.0s]'>
            <NavbarLink route='/projects' display='Projects' />
        </inline>
        <inline class='flex flex-col {itemClass} transition-[opacity] ease-in-out duration-[1.25s]'>
            <NavbarLink route='/resume' display='Resume' />
        </inline>
    </div>
</div>