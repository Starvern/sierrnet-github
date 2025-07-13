<script>
    import { page } from '$app/state';

    let currentRoute = $derived(page.route.id);
    let {route, display} = $props();
    let routeMatches = $derived(currentRoute == route);
    let classes = $derived(routeMatches ? 'text-sky-400 bg-[#1f1c26]' : 'hover:text-sky-300 hover:bg-[#1b1821]');
</script>

<a href='{route}' class='peer transition duration-[0.25s] {classes} w-full text-center p-2 h-full z-1'>
    {display}
</a>
    