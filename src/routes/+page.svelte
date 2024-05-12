<script>
    import featured_article from '$lib/images/featured-article.png';
    import boquet_left from '$lib/images/boquet-left.png';
    import boquet_right from '$lib/images/boquet-right.png';
    import boquet_up from '$lib/images/boquet-up.png';
    import boquet_down from '$lib/images/boquet-down.png';
    import tear_south_sm_white from '$lib/images/tear-south-sm-white.png';
    import tear_south_sm_offwhite from '$lib/images/tear-south-sm-offwhite.png';
    
    import SectionWrapper from '$lib/components/SectionWrapper.svelte';
    import CardWrapper from '$lib/components/CardWrapper.svelte';

</script>

<SectionWrapper>
    <div class="relative z-40 flex flex-row justify-center py-4">
        <div class="flex items-center -mr-32 desktop max-w-80">
            <img src={boquet_left} alt="">
        </div>
        <div class="flex flex-col items-center justify-center max-w-96">
            <CardWrapper>
                <div class="relative z-50 px-8 py-4 bg-white">
                    <h1 class="pb-6 text-5xl font-bold">retail therapy.</h1>
                    <h2 class="pb-3 font-medium text-md "><span class="italic font-bold">blog</span>  •  by  •  YSABEL DINSAY</h2>
                    <h2 class="pb-5 font-medium text-md">re•tail ther•a•py    ||    /ˈrē-ˌtāl ˈTHerəpē/</h2>
                    <p class="text-xl font-medium">a monthly blog focused on making you a smarter consumer one story at a time.</p>
                </div>
            </CardWrapper>
        </div>
        <div class="flex items-center -ml-32 desktop max-w-80">
            <img src={boquet_right} alt="">
        </div>
    </div>
</SectionWrapper>

<section class="my-4">
    <div class="md:-mt-16 lg:-mt-16 md:flex md:flex-row md:justify-center">
        <div class="justify-center mb-4 md:my-4 md:mx-8 md:max-w-96">
            <img class="relative z-50 mx-auto -mb-32 max-w-72 md:max-w-none md:px-8" src={featured_article} alt="">
            <img class="z-10 tear-north-sm" src={tear_south_sm_offwhite} alt="">
            <div class="relative z-40 px-8 pt-24 lg:px-12 bg-offwhite">
                <h1 class="pb-6 text-2xl">“I did a thing:” The science behind your impulse buys</h1>
                <p class="pb-6 text-sm">Last week, I walked into an Adidas to kill some time. I like to work out and it was time to buy a more supportive sports bra soon. Time to canvas, I thought. So I walk into the women’s section and that’s when I see it in my favorite shade of muted blue. I read the tag and like it’s fate, I see the words “high-support.” It’s just what I need – but wait...</p>
                <a class="text-2xl" href="articles/impulse_buy"><div class="text-center text-white w-44 hover:underline bg-offblack border-[0.5rem] border-offblack">read more</div></a>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_offwhite} alt="">
        </div>

        <div class="justify-center mt-4 md:my-4 md:mx-8 md:max-w-96">
            <img class="relative z-50 mx-auto -mb-32 max-w-72 md:max-w-none md:px-8" src={featured_article} alt="">
            <img class="z-10 tear-north-sm" src={tear_south_sm_offwhite} alt="">
            <div class="relative z-40 px-8 pt-24 lg:px-12 bg-offwhite">
                <h1 class="pb-6 text-2xl">“I did a thing:” The science behind your impulse buys</h1>
                <p class="pb-6 text-sm">Last week, I walked into an Adidas to kill some time. I like to work out and it was time to buy a more supportive sports bra soon. Time to canvas, I thought. So I walk into the women’s section and that’s when I see it in my favorite shade of muted blue. I read the tag and like it’s fate, I see the words “high-support.” It’s just what I need – but wait...</p>
                <a class="text-2xl" href="articles/impulse_buy"><div class="text-center text-white w-44 hover:underline bg-offblack border-[0.5rem] border-offblack">read more</div></a>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_offwhite} alt="">
        </div>
    </div>
</section>

<SectionWrapper>
    <div class="py-6 overflow-clip md:flex md:justify-center bg-offwhite">
        <div class="justify-center mx-auto mt-4 -mb-32 md:-mb-0 max-w-96 md:my-4 md:mx-8">
            <img class="relative z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-40 px-8 bg-white lg:px-12">
                <h1 class="pb-6 text-2xl">“I did a thing:” The science behind your impulse buys</h1>
                <p class="text-sm">Last week, I walked into an Adidas to kill some time. I like to work out and it was time to buy a more supportive sports bra soon. Time to canvas, I thought. So I walk into the women’s section and that’s when I see it in my favorite shade of muted blue. I read the tag and like it’s fate, I see the words “high-support.” It’s just what I need – but wait...</p>
            </div>
            <img class="relative z-10 tear-south-sm" src={tear_south_sm_white} alt="">
            <img class="z-0 -mt-32 -ml-24 md:ml-20" src={boquet_down} alt="">
        </div>

        <div class="justify-center pb-32 mx-auto mt-4 -mb-32 md:pb-0 md:-mb-0 max-w-96 md:my-4 md:mx-8">
            <img class="z-0 w-full ml-24 -mb-40 md:-ml-20" src={boquet_up} alt="">
            <img class="relative z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-40 px-8 bg-white lg:px-12">
                <h1 class="pb-6 text-2xl">“I did a thing:” The science behind your impulse buys</h1>
                <p class="text-sm">Last week, I walked into an Adidas to kill some time. I like to work out and it was time to buy a more supportive sports bra soon. Time to canvas, I thought. So I walk into the women’s section and that’s when I see it in my favorite shade of muted blue. I read the tag and like it’s fate, I see the words “high-support.” It’s just what I need – but wait...</p>
            </div>
            <img class="relative z-10 tear-south-sm" src={tear_south_sm_white} alt="">
        </div>
    </div>
</SectionWrapper>

<style>
    /* your styles go here */

    /*
    .shadow {
        filter: drop-shadow(0 0.1rem 0.2rem black);
    }
    */

    @media(max-width: 425px) {
        .desktop {
            display: none;
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

    /*
    h1 {
        font-size: 2rem;
        line-height: 3rem;
    }

    p {
        font-size: 1rem;
        line-height: 1.5rem;
    } */
</style>