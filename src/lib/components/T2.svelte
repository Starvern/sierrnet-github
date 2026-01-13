<script lang="ts">
    let { children, ...data } = $props();
</script>

<h2 class='text-[1rem] text-center md:text-left md:text-[1.5rem] {data.class}'>
    {@render children?.()}
</h2>