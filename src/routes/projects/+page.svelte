<script>
    import BlockText from "$lib/BlockText.svelte";
    import BlockTitle from "$lib/BlockTitle.svelte";
    import DisplayBlock from "$lib/DisplayBlock.svelte";
    import PageTitle from "$lib/PageTitle.svelte";
</script>

<PageTitle>Projects</PageTitle>

<DisplayBlock>
    <BlockTitle>
        <a href="https://github.com/Starvern/UltimateUserInterface" class='text-sky-200 underline'>
            UltimateUserInterface
        </a>
    </BlockTitle>
    <BlockText>A GUI library for plugin developers and server administrators for Spigot server software.</BlockText>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>
        <a href="https://github.com/Starvern/rust-auth" class='text-sky-200 underline'>
            rust-auth
        </a>
    </BlockTitle>
    <BlockText>A REST username-password authentication service written in Rust.</BlockText>
</DisplayBlock>

<PageTitle>Source Code</PageTitle>

<DisplayBlock>
    <BlockTitle>
        <a href="https://github.com/Starvern/sierrnet-github" class='text-sky-200 underline'>
            sierrnet-github
        </a>
    </BlockTitle>
    <BlockText>View the source for this website.</BlockText>
</DisplayBlock>