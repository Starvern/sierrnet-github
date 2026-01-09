<script>
    import BlockText from "$lib/components/BlockText.svelte";
    import BlockTitle from "$lib/components/BlockTitle.svelte";
    import DisplayBlock from "$lib/components/DisplayBlock.svelte";
    import PageTitle from "$lib/components/PageTitle.svelte";
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
        <a href="https://github.com/Starvern/hack-midwest-2025" class='text-sky-200 underline'>
            RepEngine - hack-midwest-2025
        </a>
    </BlockTitle>
    <BlockText>
        My entry for HackMidest 2025. Using MongoDB & Sveltekit to create a workout app which uses MongoDB's vector search
        to suggest workouts based on user data.
    </BlockText>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>
        <a href="https://github.com/Starvern/mcp-led-controller" class='text-sky-200 underline'>
            mcp-led-controller
        </a>
    </BlockTitle>
    <BlockText>A three-part system with an MCP server, WebSocket server, and Arduino WebSocket client. This system can use AI models to toggle an LED on and off.</BlockText>
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