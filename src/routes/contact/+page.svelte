<script>
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';

    import boquet_left from '$lib/images/boquet-left.png';

    import SectionWrapper from '$lib/components/SectionWrapper.svelte';
    import CardWrapper from '$lib/components/CardWrapper.svelte';
</script>

<SectionWrapper>
    <div class="flex justify-center py-4">
        <div class="relative z-0 hidden max-w-xs my-auto -mr-32 min-[425px]:block">
            <img src={boquet_left} alt="">
        </div>
        <div class="relative z-10 max-w-sm my-auto">
            <CardWrapper>
                <div class="p-8">
                    <h1 class="pb-6 text-3xl">Let's talk!</h1>
                    <p class="pb-4 text-sm text-justify">
                        If you have a project idea in mind, please get in touch. 
                        <br>
                        I will be happy to discuss ideas with you and how we can work together.
                        <br>
                        If you’d like to reach out, feel free to send an email or contact me via my social media channels.
                    </p>
                    <div class="text-center">
                        <a class="mt-2 text-sm text-center hover:underline" href="mailto:maria.ysabel.dinsay@gmail.com">maria.ysabel.dinsay@gmail.com</a>
                    </div>
                    <div class="flex justify-center">
                        <a class="mx-2 mt-4 size-6" href="https://www.linkedin.com/in/ysabel-dinsay/"><img src={linkedin_icon_graphic} alt="Linkedin logo"></a>
                        <a class="mx-2 mt-4 size-6" href="https://www.instagram.com/ysabeldinsay/"><img src={ig_icon_graphic} alt="Instagram logo"></a>
                    </div>
                </div>
            </CardWrapper>
        </div>
        <div class="relative z-0 hidden max-w-xs my-auto -ml-32 min-[425px]:block">
            <img class="-scale-x-100" src={boquet_left} alt="">
        </div>
    </div>
</SectionWrapper>