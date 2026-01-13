<script lang="ts">
    let { children, ...data } = $props();
</script>

<div class='border-t-[0.125rem] border-dashed border-stone-300 px-[2rem] pt-[2rem] {data.class}'>
    {@render children?.()}
</div>
