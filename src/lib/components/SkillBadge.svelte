<script lang="ts">
    import T2 from '$lib/components/T2.svelte';

    let { children, icon = "", ...data } = $props();
</script>


<T2 class='w-full h-full {data.class}'>
    <i class={icon}></i>
    {@render children?.()}
</T2>