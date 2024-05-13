<script>
    import featured_article from '$lib/images/featured-article.png';
    import boquet_right from '$lib/images/bouquet-sunflower-right.png';
    import tear_south_sm_white from '$lib/images/tear-south-sm-white.png';
    
    import SectionWrapper from '$lib/components/SectionWrapper.svelte';
</script>

<SectionWrapper>
    <div class="py-2 mx-auto md:py-0 md:grid md:grid-cols-12 md:max-w-4xl">
        <div class="z-10 my-auto md:col-start-2 md:col-end-10 md:row-start-1 md:row-end-1">
            <img class="relative z-0 tear-north-base" src={tear_south_sm_white} alt="">
            <div class="relative z-50 bg-white md:flex md:justify-center">
                <div class="mx-8 md:mx-0 md:my-auto md:-ml-8">
                    <img class="" src={featured_article} alt="">
                </div>
                <div class="p-4 md:pl-2 md:pr-4 md:flex md:flex-col md:justify-center">
                    <h1 class="pb-4 text-2xl">“I did a thing:” The science behind your impulse buys</h1>
                    <p class="pb-4 text-sm">Last week, I walked into an Adidas to kill some time. I like to work out and it was time to buy a more supportive sports bra soon. Time to canvas, I thought. So I walk into the women’s section and that’s when I see it in my favorite shade of muted...</p>
                    <a class="text-lg" href="articles/impulse-buy"><div class="text-center text-white border-2 w-36 hover:underline bg-offblack border-offblack">read more</div></a>
                </div>
            </div>
            <img class="relative z-10 tear-south-base" src={tear_south_sm_white} alt="">
        </div>
        <div class="z-0 hidden my-auto md:col-start-8 md:col-end-13 md:row-start-1 md:row-end-1 md:block">
            <img class="" src={boquet_right} alt="">
        </div>
    </div>
    
    <div class="md:flex md:flex-row md:justify-center">
        <div class="justify-center md:my-4 md:mx-8 md:max-w-72">
            <div class="pb-6 mx-8">
                <img class="relative z-50 max-w-xs mx-auto -mb-32 md:max-w-none" src={featured_article} alt="">
            </div>
            <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-40 p-4 pt-24 bg-white">
                <h1 class="pb-4 text-lg">“I did a thing:” The science behind your impulse buys</h1>
                <a class="text-lg" href="articles/impulse-buy"><div class="text-center text-white border-2 w-36 hover:underline bg-offblack border-offblack">read more</div></a>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
        </div>

        <div class="justify-center md:my-4 md:mx-8 md:max-w-72">
            <div class="pb-6 mx-8">
                <img class="relative z-50 max-w-xs mx-auto -mb-32 md:max-w-none" src={featured_article} alt="">
            </div>
            <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-40 p-4 pt-24 bg-white">
                <h1 class="pb-4 text-lg">“I did a thing:” The science behind your impulse buys</h1>
                <a class="text-lg" href="articles/impulse-buy"><div class="text-center text-white border-2 w-36 hover:underline bg-offblack border-offblack">read more</div></a>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
        </div>

        <div class="justify-center md:my-4 md:mx-8 md:max-w-72">
            <div class="pb-6 mx-8">
                <img class="relative z-50 max-w-xs mx-auto -mb-32 md:max-w-none" src={featured_article} alt="">
            </div>
            <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-40 p-4 pt-24 bg-white">
                <h1 class="pb-4 text-lg">“I did a thing:” The science behind your impulse buys</h1>
                <a class="text-lg" href="articles/impulse-buy"><div class="text-center text-white border-2 w-36 hover:underline bg-offblack border-offblack">read more</div></a>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
        </div>
    </div>
</SectionWrapper>

<style>
    .tear-south-base {
        background-color: transparent;

        margin-top: -2.5rem;

        @media(min-width: 768px) {
            margin-top: -5rem;
        }

        @media(min-width: 1024px) {
            margin-top: -5rem;
        }
    }

    .tear-north-base {
        transform: rotate(180deg);

        background-color: transparent;

        margin-bottom: -2.5rem;

        @media(min-width: 768px) {
            margin-bottom: -5rem;
        }

        @media(min-width: 1024px) {
            margin-bottom: -5rem;
        }
    }

    .tear-south-sm {
        background-color: transparent;

        margin-top: -1rem;

        @media(min-width: 768px) {
            margin-top: -1rem;
        }

        @media(min-width: 1024px) {
            margin-top: -1.5rem;
        }
    }

    .tear-north-sm {
        transform: rotate(180deg);

        background-color: transparent;

        margin-bottom: -1rem;

        @media(min-width: 768px) {
            margin-bottom: -1rem;
        }

        @media(min-width: 1024px) {
            margin-bottom: -1.5rem;
        }
    }

    img {
        font-style: italic;

        background-repeat: no-repeat;
        background-size: cover;

        width: 100%;
        height: auto;
            
        vertical-align: middle;
    }
</style>