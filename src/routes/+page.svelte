<script lang="ts">
    import StarvernKnightPurple from "$lib/assets/StarvernKnightPurple.png";
    import lasermaze from "$lib/assets/lasermaze.jpg";
    import DisplaySection from '$lib/components/DisplaySection.svelte';
    import T1 from '$lib/components/T1.svelte';
    import T2 from '$lib/components/T2.svelte';
    import SocialLink from '$lib/components/SocialLink.svelte';
    import T3 from '$lib/components/T3.svelte';
    import InlineSection from '$lib/components/InlineSection.svelte';
    import resume from '$lib/Resume.pdf';
    </script>

<DisplaySection class='flex flex-col md:flex-row md:gap-20'>
    <img class="animate-set w-60 h-60 self-center md:mt-0 md:w-[20rem] md:h-80" src={StarvernKnightPurple} alt=StarvernKnightPurple />
    <div class='flex flex-col md:py-10 animate-set'>
        <T1>Hi, I'm William</T1>
        <T2>Junior B.S. Computer Engineering @ Univeristy of Kansas</T2>

        <T3 class='text-stone-500 mt-4'>
            <i>I'm a student from Kansas City exploring avionics and RF systems through my work and coursework.</i>
        </T3>

        <div class='text-[2.5rem] text-stone-500 mx-auto md:mx-0 py-4'>
            <SocialLink label=github link='https://github.com/Starvern' icon='fa-brands fa-github' />
            <SocialLink label=linkedin link='https://www.linkedin.com/in/william-sierra-2497b3262/' icon='fa-brands fa-linkedin' />
        </div>

        <a aria-label=resume
           download
           href={resume}
           class='border w-fit px-4 py-2 rounded-xs hover:bg-black hover:text-white transition duration-200 mx-auto mb-8 md:m-0'>
            <i class='fa-solid fa-download'></i>
            Download Resume
        </a>
    </div>
</DisplaySection>

<DisplaySection dark={false} class='border-t-2'>
	<div class='flex flex-row items-center px-8 py-7'>
	</div>
</DisplaySection>

<DisplaySection dark={true} class='p-8 leading-6 md:leading-10'>
    <T2>VIAVI Solutions (Avionics R&D) - Test Engineer Intern</T2>
    <T3 class='text-stone-600 mb-2'>Lenexa, KS - May 2026 - Present</T3>
    <ul class='text-[0.75rem] md:text-[1.25rem]'>
        <li>
            <ul>
                <li>• Automated design verification test (DVT) for the ATC5000NG</li>
                <ul class='ml-8 text-stone-600'>
                    <li>Eliminated 6+ weeks of manual testing of 60+ modules and 2000+ measurements</li>
                    <li>Introduced GUM-compliant Type A and Type B uncertainty tracking</li>
                    <li>Integrated with NI TestStand using compiled DLLs</li>
                </ul>
            </ul>
        </li>
        <li>
            <ul>
                <li>• Contributed to TestBench, the core testing framework used by the team</li>
                <ul class='ml-8 text-stone-600'>
                    <li>Used by the ATC5000NG, and will support future test programs</li>
                    <li>Currently developing tests for the successor to the AVX-10K using this framework</li>
                </ul>
            </ul>
        </li>
        <li>
            <ul>
                <li>• Migrated TestBench from C++ to C#</li>
                <ul class='ml-8 text-stone-600'>
                    <li>Allows proper integration with METAS UncLib</li>
                    <li>Saved $1,000/year per developer (from license cost)</li>
                </ul>
            </ul>
        </li>
        <li>
            <ul>
                <li>• Performed digital signal processing (DSP) analysis on RF waveforms</li>
                <ul class='ml-8 text-stone-600'>
                    <li>Measured DME and Mode S Pulse Characteristics</li>
                    <li>IQ demodulation, finite impulse response (FIR) filters, and least-squares regression</li>
                </ul>
            </ul>
        </li>
        <li>
            <ul>
                <li>• Performed precision RF measurements using calibrated instruments for tracability</li>
                <ul class='ml-8 text-stone-600'>
                    <li>R&S FSMR3008 Measuring Receiver</li>
                    <li>R&S MXO34 Oscilliscope</li>
                    <li>R&S SMBV100B Vector Signal Generator</li>
                    <li>R&S ZNB Vector Network Analyzer</li>
                    <li>Keysight DSOS204A RF Oscilliscope</li>
                </ul>
            </ul>
        </li>
    </ul>
</DisplaySection>

<DisplaySection class='py-8 pb-12 flex flex-col gap-8'>
    <T1 class='mx-8'>Education</T1>

    <InlineSection>
        <T2>University of Kansas</T2>
        <T3 class='text-stone-600'>B.S. Computer Engineering, Graduating 2028, 4.0 GPA</T3>
    </InlineSection>

    <InlineSection>
        <T2>Warrensburg High School</T2>
        <T3 class='text-stone-600'>Class of 2024, 3.84 / 4.19 GPA</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-8 pb-12 flex flex-col gap-12 md:gap-8'>
    <T1 class='mx-8'>Projects</T1>

    <InlineSection>
        <T2>Laser Maze</T2>

        <a href={lasermaze} class='text-center md:text-right'>Click here to see image.</a>
        <T3 class='text-stone-600'>I created a fully-functional laser maze within my garage using Arduino, lasers, and photoresistors.</T3>
    
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://github.com/Starvern/rf24-drone-project' label=drone>
                Custom Ground Drone
            </SocialLink>
            <T3 class='text-stone-600'>I used Arduino to create a custom ground drone, and a seperate custom radio controller.</T3>
        </T2>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://github.com/Starvern/dht-esp8266-socketio' label=drone>
                IoT Smart Home Thermometer
            </SocialLink>
            <T3 class='text-stone-600'>I used Arduino and a custom SocketIO server to create a smart-home thermometer which outputs temperature data to the server.</T3>
        </T2>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://github.com/Starvern/UltimateUserInterface' label=uui>
                UltimateUserInterface
            </SocialLink>

        </T2>
        <T3 class='text-stone-600'>A GUI library for plugin developers and server administrators for Spigot server software.</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://github.com/Starvern/hack-midwest-2025' label=hackmidwest>
                RepEngine - hack-midwest-2025
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>My entry for HackMidest 2025. Using MongoDB & Sveltekit to create a workout app which uses MongoDB's vector search to suggest workouts based on user data.</T3>
    </InlineSection>

    <InlineSection>
        <T2>
            <SocialLink link='https://github.com/Starvern/mcp-led-controller' label='mcp-led-controller' icon=''>
                mcp-led-controller
            </SocialLink>
        </T2>

        <T3 class='text-stone-600'>A three-part system with an MCP server, WebSocket server, and Arduino WebSocket client. This system can use AI models to toggle an LED on and off.</T3>
    </InlineSection>


    <InlineSection>
        <T2>
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
            <SocialLink link='https://github.com/Starvern/sierrnet-github' label=sierrnet-github>
                sierrnet-github
            </SocialLink>
        </T2>
        <T3 class='text-stone-600'>View the source for this website.</T3>
    </InlineSection>
</DisplaySection>

<DisplaySection class='py-8 pb-12 flex flex-col gap-8'>
    <T1 class='mx-8'>Awards & Competition Placements</T1>

    <InlineSection>
        <T2>Dean's List / Honor Roll - 2024, 2025, Spring 2026</T2>
        <T3 class='text-stone-600'>University of Kansas</T3>
    </InlineSection>

    <InlineSection>
        <T2>Academic Excellence - 2021, 2022, 2023, 2024</T2>
        <T3 class='text-stone-600'>Warrensburg High School</T3>
    </InlineSection>

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