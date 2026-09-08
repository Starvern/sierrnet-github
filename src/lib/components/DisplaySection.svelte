<script lang="ts">
    let { children, dark = false, ...data } = $props();

    const dark_class = "text-stone-300 bg-[linear-gradient(to_left,#1c1917,#0c0a09)] before:content-[\'\'] before:absolute before:inset-0 before:pointer-events-none before:bg-[linear-gradient(#ffffff08_1px,transparent_1px),linear-gradient(90deg,#ffffff08_1px,transparent_1px),radial-gradient(circle_at_25%_20%,#22c55e0d,transparent_60%)] before:bg-size-[20px_20px,20px_20px,100%_100%] before:mask-[linear-gradient(to_right,transparent,black_12%,black_88%,transparent)] before:[-webkit-mask-image:linear-gradient(to_right,transparent,black_12%,black_88%,transparent)]"
</script>

<div class='md:px-[10%] relative {dark
    ? dark_class
    : "border-stone-300 bg-[radial-gradient(circle,#00000025_1px,transparent_1px)] bg-size-[20px_20px]"}'>
    <div class='{dark ? "" : "md:border-x-2 md:border-stone-300"} {data.class} relative'>
        {@render children?.()}
    </div>
</div>