<script>
    import DisplaySection from '$lib/components/DisplaySection.svelte';
    import T1 from '$lib/components/T1.svelte';
    import T2 from '$lib/components/T2.svelte';
    import T3 from '$lib/components/T3.svelte';
    import StarvernKnightGif from '$lib/assets/StarvernKnightGif.gif';
    import SocialLink from '$lib/components/SocialLink.svelte';
    import WaccEsportsOld from '$lib/assets/WaccEsportsOld.png';
    import WaccEsportsNew from '$lib/assets/WaccEsportsNew.png';

    import StarforgeLogo from '$lib/assets/StarforgeLogo.png';
    import StarforgeText from '$lib/assets/StarforgeText.png';

    import dark_etherium from "$lib/assets/icons/dark_etherium.gif"
    import onyx from "$lib/assets/icons/onyx.gif"
    import opal from "$lib/assets/icons/opal.gif"
    import pure_etherium from "$lib/assets/icons/pure_etherium.gif"
    import pure_etherium_pickaxe from "$lib/assets/icons/pure_etherium_pickaxe.gif"
    import pure_etherium_sword from "$lib/assets/icons/pure_etherium_sword.gif"
    import raw_etherium from "$lib/assets/icons/raw_etherium.gif"
    import refined_etherium from "$lib/assets/icons/refined_etherium.gif"
    import resume from '$lib/Resume.pdf';
</script>

<DisplaySection class='flex flex-col md:flex-row md:gap-[5rem]'>
    <img class="animate-set w-[15rem] h-[15rem] self-center md:mt-0 md:w-[20rem] md:h-[20rem]" src={StarvernKnightGif} alt=StarvernKnightPurple />
    <div class='flex flex-col md:py-[2.5rem] animate-set'>
        <T1>My Design Portfolio</T1>
        <T2>Sophomore B.S. Computer Engineering @ Univeristy of Kansas</T2>

        <div class='text-[2.5rem] text-stone-500 mx-auto md:mx-0 py-[1rem]'>
            <SocialLink label=github link='https://github.com/Starvern' icon='fa-brands fa-github' />
            <SocialLink label=linkedin link='https://www.linkedin.com/in/william-sierra-2497b3262/' icon='fa-brands fa-linkedin' />
        </div>
        <a aria-label=resume
           download
           href={resume}
           class='border-1 w-fit px-[1rem] py-[0.5rem] rounded-xs hover:bg-black hover:text-white transition duration-200 mx-auto mb-[2rem] md:m-0'>
            <i class='fa-solid fa-download'></i>
            Download Resume
        </a>
    </div>
</DisplaySection>

<DisplaySection dark={true} class='pt-[2rem]'>
    <T2 class='mx-[2rem]'>Wooden Furniture</T2>
    <T3 class='mx-[2rem] mb-[2rem]'>
        100% Custom Models and Textures. These were made under my psuedonym "Starvern" for the brand "Light Designs"
    </T3>
    <iframe
        title="Wooden Furniture"
        allowfullscreen
        allow="autoplay; fullscreen; xr-spatial-tracking"
        src="https://sketchfab.com/models/f47efdb78d3642d5ac955a65fc58f2db/embed?ui_theme=dark"
        class="h-[40rem] w-full"
    >
    </iframe>
</DisplaySection>

<DisplaySection dark={true} class='pt-[2rem] pb-[3rem]'>
    <T2 class='mx-[2rem]'>Tiger / WACC Esports</T2>
    <T3 class='mx-[2rem] text-stone-400'>I created this logo for the newly founded esports team in the Warrensburg School District. </T3>
    <T3 class='mx-[2rem] text-stone-400 mb-[2rem]'>The first one was my initial attempt and after recieving some feedback, I designed the second one.</T3>
    <div class='flex flex-col xl:flex-row items-center justify-center gap-[2rem] xl:gap-[10rem]'>
        <img class='w-[30rem]' src={WaccEsportsOld} alt=wacc_old />
        <img class='w-[30rem]' src={WaccEsportsNew} alt=wacc_new />
    </div>
</DisplaySection>

<DisplaySection dark={true} class='pt-[2rem] pb-[3rem]'>
    <T2 class='mx-[2rem]'>Starforge</T2>
    <T3 class='mx-[2rem] text-stone-400 mb-[2rem]'>I publish all my models and pixelart under this shop. This style is video-game/pixelart.</T3>
    <div class='flex flex-col xl:flex-row items-center justify-center gap-[2rem] xl:gap-[10rem]'>
        <img class='w-[30rem] pixel-perfect' src={StarforgeLogo} alt=wacc_old />
        <img class='w-[30rem] pixel-perfect' src={StarforgeText} alt=wacc_new />
    </div>
</DisplaySection>

<DisplaySection dark={true} class='pt-[2rem] pb-[3rem]'>
    <T2 class='mx-[2rem]'>Pixel Art Icons</T2>
    <T3 class='mx-[2rem] mb-[2rem]'>Here are a few pixel art icons I've made.</T3>

    <div class='md:mx-[2rem] content-center w-full grid grid-cols-2 md:grid-cols-3 xl:grid-cols-5 gap-[1rem]'>
        <img src={dark_etherium} alt=dark_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={onyx} alt=onyx class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={opal} alt=opal class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium} alt=pure_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium_pickaxe} alt=pure_etherium_pickaxe class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={pure_etherium_sword} alt=pure_etherium_sword class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={raw_etherium} alt=raw_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
        <img src={refined_etherium} alt=refined_etherium class='w-[10rem] h-[10rem] pixel-perfect'/>
    </div>

</DisplaySection>

<style>
    .pixel-perfect {
        image-rendering: pixelated;
    }
</style>