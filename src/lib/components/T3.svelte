<script lang="ts">
    let { children, ...data } = $props();
</script>

<h3 class='text-[0.9rem] text-center md:text-left md:text-[1.25rem] {data.class}'>
    {@render children?.()}
</h3>