<script>
    import resume from '$lib/Resume.pdf'
    import passport from '$lib/Passport.pdf'
    import DisplayBlock from '$lib/DisplayBlock.svelte';
    import ListElement from '$lib/ListElement.svelte';
    import PageTitle from '$lib/PageTitle.svelte';
    import BlockSubtitle from '$lib/BlockSubtitle.svelte';
    import BlockTitle from '$lib/BlockTitle.svelte';
</script>

<PageTitle>
    <inline>Resume</inline>
    <a href={resume} download class='bg-[#131116] text-sky-200 text-[1.5rem] align-middle p-[0.5rem]'>
        Download
    </a>
</PageTitle>

<PageTitle>Experience</PageTitle>

<DisplayBlock>
    <BlockTitle>Warrensburg R-VI School District - I.T. Support Internship</BlockTitle>
    <BlockSubtitle>Warrensburg, MO - September 2023 - May 2024</BlockSubtitle>
    <ListElement>Running eternet cables from devices such as TV's, Raspberry pi's, and access points to network switches</ListElement>
    <ListElement>Responding to various tickets issued by teachers, office staff, etc.</ListElement>
    <ListElement>Projecter, printer, and screen setup inside classrooms and offices</ListElement>
    <ListElement>Repairing student and faculty laptops</ListElement>
    <ListElement>Salvaged damaged laptops for working components used in future repairs</ListElement>
</DisplayBlock>


<DisplayBlock>
    <BlockTitle>Western Missouri Medical Center - Internet Services Internship</BlockTitle>
    <BlockSubtitle>Warrensburg, MO - December 2022 - May 2023</BlockSubtitle>
    <ListElement>Terminating network cables with either male jacks or female keystones</ListElement>
    <ListElement>Installing and configuring network switches</ListElement>
    <ListElement>Communicating the problem and solution to various hospital faculty</ListElement>
    <ListElement>Reparing faculty equipment and maintaining hospital devices</ListElement>
    <ListElement>Updating and installing software on equipment</ListElement>
</DisplayBlock>

<PageTitle>Education</PageTitle>

<DisplayBlock>
    <BlockTitle>University of Kansas</BlockTitle>
    <BlockSubtitle>B.S. Computer Engineering, Expected 2028</BlockSubtitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>Warrensburg High School</BlockTitle>
    <BlockSubtitle>Class of 2024, 3.84 / 4.19 GPA</BlockSubtitle>
</DisplayBlock>

<PageTitle>Certifications</PageTitle>

<DisplayBlock>
    <BlockTitle>
        <a href='https://verification.testout.com/verifycert/6-1C6-V2SSKD' class='text-sky-200 underline'>
            CompTIA TestOut PC Pro Certification
        </a>
    </BlockTitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>
        <a href='https://verification.testout.com/verifycert/6-1C6-VFPEXB' class='text-sky-200 underline'>
            CompTIA TestOut Network Pro Certification
        </a>
    </BlockTitle>
</DisplayBlock>

<PageTitle>Awards</PageTitle>

<DisplayBlock>
    <BlockTitle>
        <a href='https://news.ku.edu/university-kansas-fall-2024-honor-roll-kansas-students' class='text-sky-200 underline'>
            Honor Roll - 2024
        </a>
    </BlockTitle>
    <BlockSubtitle>University of Kansas</BlockSubtitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>Academic Excellence - 2021, 2022, 2023, 2024</BlockTitle>
    <BlockSubtitle>Warrensburg High School</BlockSubtitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>
        <a href={passport} download class='text-sky-200 underline'>
                Passport Award
        </a>
    </BlockTitle>
    <BlockSubtitle>Warrensburg Area Career Center</BlockSubtitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>SkillsUSA Statesmanship and Leadership</BlockTitle>
</DisplayBlock>

<PageTitle>Competition Placement</PageTitle>

<DisplayBlock>
    <BlockTitle>
        <a href='https://www.skillsusa-register.org/rpts/EventMedalists.aspx' class='text-sky-200 underline'>
            SkillsUSA MO State Medalist
        </a>
    </BlockTitle>
    <BlockSubtitle>3rd Place Computer Programming - Apr. 2023</BlockSubtitle>
</DisplayBlock>

<DisplayBlock>
    <BlockTitle>SkillsUSA MO West-Central District Champion</BlockTitle>
    <BlockSubtitle>1st Place I.T. Services - Nov. 2023</BlockSubtitle>
</DisplayBlock>