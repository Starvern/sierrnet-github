<script lang="ts">
    let { children, dark = false, ...data } = $props();
</script>

<div class='md:px-[10%] border-b-[0.125rem] {dark ? "text-stone-300 bg-gradient-to-l from-stone-900 to-stone-950 border-stone-500" : "border-stone-300"}'>
    <div class='md:border-x-[0.125rem] {dark ? "md:border-stone-800" : "md:border-stone-300"} {data.class}'>
        {@render children?.()}
    </div>
</div>