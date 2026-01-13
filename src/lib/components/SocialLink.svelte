<script lang="ts">
    import { resolve } from '$app/paths';

    let { link, label, icon = "", children = null, download = false, ...data } = $props();

    const checkLink = (link: "/") => {
        if (link.startsWith("https://"))
            return link;

        return resolve(link)
    }

</script>

{#if download}
    <a href={checkLink(link)}
       aria-label={label}
       download
       class='{icon} hover:bg-gradient-to-t from-sky-900 to-sky-400 transition duration-100
       hover:text-transparent hover:drop-shadow-sky-200 hover:drop-shadow-xl bg-clip-text cursor-pointer {data.class}'
    >
        {@render children?.()}
    </a>
{:else}
    <a href={checkLink(link)}
       aria-label={label}
       class='{icon} hover:bg-gradient-to-t from-sky-900 to-sky-400 transition duration-100
       hover:text-transparent hover:drop-shadow-sky-200 hover:drop-shadow-xl bg-clip-text cursor-pointer {data.class}'
    >
        {@render children?.()}
    </a>
{/if}