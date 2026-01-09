<script lang="ts">
    import PageTitle from "$lib/components/PageTitle.svelte";
    import DisplayBlock from "$lib/components/DisplayBlock.svelte";
    import BlockTitle from "$lib/components/BlockTitle.svelte";
    import BlockText from "$lib/components/BlockText.svelte";
    import StarvernKnightPurple from "$lib/assets/StarvernKnightPurple.png";
    import StarvernKnightGif from "$lib/assets/StarvernKnightGif.gif";
    import TigersEsportsOld from "$lib/assets/TigersEsportsOld.png";
    import WaccEsportsFull from "$lib/assets/WaccEsportsFull.png";
    import StarforgeLogo from "$lib/assets/StarforgeLogo.png";
    import StarforgeText from "$lib/assets/StarforgeText.png";
    import dark_etherium from "$lib/assets/icons/dark_etherium.gif"
    import onyx from "$lib/assets/icons/onyx.gif"
    import opal from "$lib/assets/icons/opal.gif"
    import pure_etherium from "$lib/assets/icons/pure_etherium.gif"
    import pure_etherium_pickaxe from "$lib/assets/icons/pure_etherium_pickaxe.gif"
    import pure_etherium_sword from "$lib/assets/icons/pure_etherium_sword.gif"
    import raw_etherium from "$lib/assets/icons/raw_etherium.gif"
    import refined_etherium from "$lib/assets/icons/refined_etherium.gif"
</script>

<PageTitle>Design Portfolio</PageTitle>

<DisplayBlock>
    <BlockTitle>Wooden Furniture - Game Assets</BlockTitle>
    <BlockText>100% Custom Models and Textures. These were made under my psuedonym "Starvern" for the brand "Light Designs".</BlockText>
    <iframe
        title="Wooden Furniture"
        allowfullscreen
        allow="autoplay; fullscreen; xr-spatial-tracking"
        src="https://sketchfab.com/models/f47efdb78d3642d5ac955a65fc58f2db/embed?ui_theme=dark"
        class="h-[20rem] md:h-[50rem] mt-[1rem]"
    >
    </iframe>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>Knight Helmets</BlockTitle>
    <BlockText>Made using Adobe Photoshop in the esports logo style. I use these as online avatars.</BlockText>
    <div class='flex flex-col xl:flex-row'>
        <img src={StarvernKnightPurple} alt=knight_purple class='w-[50rem]' />
        <img src={StarvernKnightGif} alt=knight_gif class='w-[50rem]'/>
    </div>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>Tigers Esports</BlockTitle>
    <BlockText>I created this logo for the newly founded esports team in the Warrensburg School District.</BlockText>
    <BlockText>The first one was my initial attempt and after recieving some feedback, I designed the second one.</BlockText>
    <div class='flex flex-col xl:flex-row'>
        <img src={TigersEsportsOld} alt=tigers_logo_old class='w-[50rem]'/>
        <img src={WaccEsportsFull} alt=tigers_logo class='w-[50rem]'/>
    </div>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>StarForge</BlockTitle>
    <BlockText>I publish all my models and pixelart under this shop. This style is video-game/pixelart.</BlockText>
    <div class='flex flex-col md:flex-row items-center mx-auto'>
        <img src={StarforgeLogo} alt=tigers_logo_old class='w-[20rem] md:w-[50rem] aspect-auto pixel-perfect'/>
        <img src={StarforgeText} alt=tigers_logo class='w-[30rem] md:w-[50rem] aspect-auto pixel-perfect'/>
    </div>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>Various Pixelart Icons</BlockTitle>
    <BlockText>I have many pixelart icons I've made, here are a some.</BlockText>
    <div class='grid grid-cols-2 lg:grid-cols-10'>
        <img src={dark_etherium} alt=dark_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={onyx} alt=onyx class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={opal} alt=opal class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium} alt=pure_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium_pickaxe} alt=pure_etherium_pickaxe class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium_sword} alt=pure_etherium_sword class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={raw_etherium} alt=raw_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={refined_etherium} alt=refined_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
    </div>
</DisplayBlock>

<style>
    .pixel-perfect {
        image-rendering: pixelated;
    }
</style>