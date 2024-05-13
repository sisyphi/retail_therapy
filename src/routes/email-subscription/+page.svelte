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
                    <h1 class="pb-6 text-3xl">Thanks for subscribing!</h1>
                    <p class="pb-4 text-justify">
                        We'll let you know of any new articles or exciting announcements.
                    </p>
                    <div class="pb-4">
                        <a class="text-center hover:underline" href="/">go back to the home menu.</a>
                    </div>
                </div>
            </CardWrapper>
        </div>
        <div class="relative z-0 hidden max-w-xs my-auto -ml-32 min-[425px]:block">
            <img class="-scale-x-100" src={boquet_left} alt="">
        </div>
    </div>
</SectionWrapper>