<script lang="ts">
    import StarvernKnightPurple from "$lib/assets/StarvernKnightPurple.png";
    import mongodb from "$lib/assets/mongodb.svg";
    import svelte from "$lib/assets/svelte.svg";
    import blockbench from "$lib/assets/blockbench.svg";
    import DisplaySection from '$lib/components/DisplaySection.svelte';
    import T1 from '$lib/components/T1.svelte';
    import T2 from '$lib/components/T2.svelte';
    import SocialLink from '$lib/components/SocialLink.svelte';
    import T3 from '$lib/components/T3.svelte';
    import SkillBadge from '$lib/components/SkillBadge.svelte';
    import InlineSection from '$lib/components/InlineSection.svelte';
    import resume from '$lib/Resume.pdf';
    import passport from '$lib/Passport.pdf';
</script>

<DisplaySection class='flex flex-col md:flex-row md:gap-[5rem]'>
    <img class="animate-set w-[15rem] h-[15rem] self-center md:mt-0 md:w-[20rem] md:h-[20rem]" src={StarvernKnightPurple} alt=StarvernKnightPurple />
    <div class='flex flex-col md:py-[2.5rem] animate-set'>
        <T1>Hi, I'm William</T1>
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

<DisplaySection dark={true} class='p-[2rem] leading-[1.5rem] md:leading-[2.5rem]'>
    <T3>
        I'm a student from Kansas City who got their start during high school creating Discord bots in Python and Minecraft plugins in Java.
        In the hardware realm, I've made many projects with Arduino and Raspberry Pi.
        From there I've made REST APIs and websites using SvelteKit and Rust.
        Using my experience, I placed 3rd in a SkillsUSA Missouri State programming competition.
    </T3>
</DisplaySection>


<DisplaySection class='p-[2rem] pb-[3rem] flex flex-col gap-[1.5rem]'>
    <T1>Skills</T1>
    <div class='grid grid-rows-2 lg:grid-cols-2 xl:grid-cols-3 gap-[1.5rem] gap-x-[5rem]'>
        <SkillBadge icon='fa-brands fa-python'>Python (4 years)</SkillBadge>
        <SkillBadge icon='fa-brands fa-java'>Java (3 years)</SkillBadge>
        <SkillBadge icon='fa-brands fa-js'>JavaScript (2 years)</SkillBadge>
        <SkillBadge><img class='w-[1.5rem] inline' src={mongodb} alt=mongodb /> MongoDB (2 years)</SkillBadge>
        <SkillBadge><img class='w-[1.5rem] inline' src={svelte} alt=svelte /> SvelteKit (2 years)</SkillBadge>
        <SkillBadge><img class='w-[1.5rem] inline' src={blockbench} alt=svelte /> Blockbench (2 years)</SkillBadge>
        <SkillBadge icon='fa-brands fa-rust'>Rust (learning)</SkillBadge>
        <SkillBadge icon='fa-brands fa-git-alt'>Git CLI (learning)</SkillBadge>
    </div>
</DisplaySection>


<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[3rem]'>
    <T1 class='px-[2rem]'>Experience</T1>

    <InlineSection>
        <T2>Warrensburg R-VI School District - I.T. Internship</T2>
        <T3 class='text-stone-600 mb-[0.5rem]'>Warrensburg, MO - September 2023 - May 2024</T3>
        <ul class='text-[0.75rem] md:text-[1.25rem]'>
            <li>• Running eternet cables from devices such as TV's, Raspberry pi's, and access points to network switches</li>
            <li>• Responding to various tickets issued by teachers, office staff, etc.</li>
            <li>• Projecter, printer, and screen setup inside classrooms and offices</li>
            <li>• Repairing student and faculty laptops</li>
            <li>• Salvaged damaged laptops for working components used in future repairs</li>
        </ul>
    </InlineSection>

    <InlineSection>
        <T2>Western Missouri Medical Center - I.T. Internship</T2>
        <T3 class='text-stone-600 mb-[0.5rem]'>Warrensburg, MO - September 2023 - May 2024</T3>
        <ul class='text-[0.75rem] md:text-[1.25rem]'>
            <li>• Terminating network cables with jacks and keystones</li>
            <li>• Installing and configuring network switches</li>
            <li>• Communicating the problem and solution to various hospital faculty</li>
            <li>• Reparing faculty equipment and maintaining hospital devices</li>
            <li>• Updating and installing software on equipment</li>
        </ul>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[3rem] md:gap-[2rem]'>
    <T1 class='mx-[2rem]'>Projects</T1>

    <InlineSection>
        <T2>
            <i class='fa-brands fa-java'></i>

            <SocialLink link='https://github.com/Starvern/UltimateUserInterface' label=uui>
                UltimateUserInterface
            </SocialLink>

        </T2>
        <T3 class='text-stone-600'>A GUI library for plugin developers and server administrators for Spigot server software.</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <i class='fa-brands fa-js'></i>
            <img class='w-[1.5rem] inline' src={mongodb} alt=mongodb />
            <img class='w-[1.5rem] inline' src={svelte} alt=mongodb />

            <SocialLink link='https://github.com/Starvern/hack-midwest-2025' label=hackmidwest>
                RepEngine - hack-midwest-2025
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>My entry for HackMidest 2025. Using MongoDB & Sveltekit to create a workout app which uses MongoDB's vector search to suggest workouts based on user data.</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <i class='fa-brands fa-python'></i>
            <i class='fa-brands fa-rust'></i>
            <SocialLink link='https://github.com/Starvern/mcp-led-controller' label='mcp-led-controller' icon=''>
                mcp-led-controller
            </SocialLink>
        </T2>

        <T3 class='text-stone-600'>A three-part system with an MCP server, WebSocket server, and Arduino WebSocket client. This system can use AI models to toggle an LED on and off.</T3>
    </InlineSection>


    <InlineSection>
        <T2>
            <i class='fa-brands fa-rust'></i>

            <SocialLink link='https://github.com/Starvern/rust-auth' label=rust-auth>
                rust-auth
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>A REST username-password authentication service written in Rust.</T3>

    </InlineSection>

    <InlineSection>
        <T1>Source Code</T1>
    </InlineSection>

    <InlineSection>
        <T2>
            <img class='w-[1.5rem] inline' src={svelte} alt=mongodb />
            <SocialLink link='https://github.com/Starvern/sierrnet-github' label=sierrnet-github>
                sierrnet-github
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>View the source for this website.</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[2rem]'>
    <T1 class='mx-[2rem]'>Education</T1>

    <InlineSection>
        <T2>University of Kansas</T2>
        <T3 class='text-stone-600'>B.S. Computer Engineering, Graduating 2028, 4.0 GPA</T3>
    </InlineSection>

    <InlineSection>
        <T2>Warrensburg High School</T2>
        <T3 class='text-stone-600'>Class of 2024, 2.84 / 4.19 GPA</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[2rem]'>
    <T1 class='mx-[2rem]'>Certifications</T1>

    <InlineSection>
        <T2>
            <SocialLink link='https://verification.testout.com/verifycert/6-1C6-V2SSKD' label=pcpro>
                CompTIA TestOut PC Pro Certification
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>Issued April 2023</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://verification.testout.com/verifycert/6-1C6-VFPEXB' label=networkpro>
                CompTIA TestOut Network Pro Certification
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>Issued May 2024</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[2rem]'>
    <T1 class='mx-[2rem]'>Awards</T1>

    <InlineSection>
        <T2>Dean's List / Honor Roll - 2024, Fall 2025</T2>
        <T3 class='text-stone-600'>University of Kansas</T3>
    </InlineSection>

    <InlineSection>
        <T2>Academic Excellence - 2021, 2022, 2023, 2024</T2>
        <T3 class='text-stone-600'>Warrensburg High School</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link={passport} download={true} label=passport>Passport Award</SocialLink>
        </T2>
        <T3 class='text-stone-600'>Warrensburg Area Career Center</T3>
    </InlineSection>

    <InlineSection>
        <T2>SkillsUSA Statesmanship & Leadership</T2>
        <T3 class='text-stone-600'>SkillsUSA MO West-Central District</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-[2rem] pb-[3rem] flex flex-col gap-[2rem]'>
    <T1 class='mx-[2rem]'>Competition Placement</T1>

    <InlineSection>
        <T2>
            <SocialLink link='https://www.skillsusa-register.org/rpts/EventMedalists.aspx' label=skillsusa>
                SkillsUSA Missouri State Medalist
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>3rd Place Computer Programming - April 2023</T3>
    </InlineSection>

    <InlineSection>
        <T2>SkillsUSA MO West-Central District Champion</T2>
        <T3 class='text-stone-600'>1st Place I.T. Services - Nov. 2023</T3>
    </InlineSection>
</DisplaySection>