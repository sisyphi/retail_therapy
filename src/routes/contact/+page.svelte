<script>
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';

    import SectionWrapper from '$lib/components/SectionWrapper.svelte';
</script>

<SectionWrapper>
    <div class="relative z-50 gap-4 px-4 py-4 md:px-8 lg:px-32 xl:px-48 md:py-16 md:flex md:justify-center md:content-center md:items-center">
        <div class="flex flex-col md:w-1/3 lg:w-2/6">
            <h1 class="pb-6 text-3xl">Let's talk!</h1>
            <p class="pb-4 text-sm text-justify">If you have a project idea in mind, please get in touch.</p>
            <p class="pb-4 text-sm text-justify">I will be happy to discuss ideas with you and how we can work together.</p>
            <p class="pb-4 text-sm text-justify">If you’d like to reach out, feel free to send an email or contact me via my social media channels.</p>
            <a class="mt-2 text-sm text-center hover:underline" href="mailto:maria.ysabel.dinsay@gmail.com">maria.ysabel.dinsay@gmail.com</a>
            <div class="flex justify-center">
                <a class="m-2 my-4 size-6" href="https://www.linkedin.com/in/ysabel-dinsay/"><img src={linkedin_icon_graphic} alt="Linkedin logo"></a>
                <a class="m-2 my-4 size-6" href="https://www.instagram.com/ysabeldinsay/"><img src={ig_icon_graphic} alt="Instagram logo"></a>
            </div>
        </div>
    </div>
</SectionWrapper>
