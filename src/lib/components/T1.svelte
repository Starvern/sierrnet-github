<script lang="ts">
    let { children, ...data } = $props();
</script>

<h1 class='text-[2.25rem] text-center md:text-left md:text-[3rem] {data.class}'>
    {@render children?.()}
</h1>