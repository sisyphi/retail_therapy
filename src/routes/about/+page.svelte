<script>
    import about_me from '$lib/images/abt-me-portrait.png';
    import acads from '$lib/images/abt-me-acads.png';
    import career from '$lib/images/abt-me-career.png';
    import boquet_left from '$lib/images/boquet-left.png';
    import boquet_right from '$lib/images/boquet-right.png';
    import boquet_up from '$lib/images/boquet-up.png';
    import boquet_down from '$lib/images/boquet-down.png';
    import tear_south_base_offwhite from '$lib/images/tear-south-base-offwhite.png';
    import tear_south_sm_white from '$lib/images/tear-south-sm-white.png';
    import tear_south_sm_offwhite from '$lib/images/tear-south-sm-offwhite.png';
</script>

<section class="">
    <img class="tear-north" src={tear_south_base_offwhite} alt="">
    <div class="relative z-40 bg-[#F8F1E7] md:-mb-24">
        <div class="flex flex-col items-center justify-center max-w-2xl m-auto md:grid md:grid-cols-4">
            <div class="-mb-8 -ml-8 md:mb-8 md:-ml-32 md:col-start-1 md:col-end-4 md:row-start-1 md:row-end-2">
                <img src={about_me} alt="">
            </div>
            <div class="max-w-96 md:col-start-3 md:col-end-5 md:row-start-1 md:row-end-2">
                <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
                <div class="relative z-50 px-8 bg-white">
                    <h1 class="pb-6 text-5xl font-bold">Hi, I'm Ysa!</h1>
                    <h2 class="pb-3 font-medium text-md "><span class="italic font-bold">about me</span>  •  YSABEL DINSAY</h2>
                    <p class="text-xl font-medium">Thanks for stopping by! Here's the story of my life.</p>
                </div>
                <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
            </div>
        </div>
    </div>
    
    <div id="articles" class="relative z-40 bg-[#F8F1E7] md:-mb-24">
        <div class="relative z-50 flex flex-col items-center justify-center max-w-2xl m-auto md:-mb-24 md:grid md:grid-cols-6">
            <div class="-mb-8 md:mb-8 md:-mr-32 md:col-start-3 md:col-end-7 md:row-start-1 md:row-end-2">
                <img src={acads} alt="">
            </div>
            <div class="max-w-96 md:col-start-1 md:col-end-6 md:row-start-1 md:row-end-2">
                <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
                <div class="relative z-50 px-8 bg-white">
                    <h1 class="pb-6 text-2xl font-bold">My Academic Life</h1>
                    <p class="text-lg font-medium">I graduated summa cum laude from De La Salle University Manila with a Major in Psychology. Passionate about the human mind, I have taken up volunteer research positions at Yale University’s Early Childhood Education Center in 2016 and 2019.</p>
                </div>
                <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
            </div>
        </div>

        <div class="relative z-20 flex flex-col items-center justify-center max-w-2xl m-auto md:grid md:grid-cols-6">
            <div class="-mb-8 -mr-8 md:mb-0 md:-ml-36 md:col-start-1 md:col-end-5 md:row-start-1 md:row-end-2">
                <img src={career} alt="">
            </div>
            <div class="max-w-96 md:col-start-3 md:col-end-8 md:row-start-1 md:row-end-2">
                <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
                <div class="relative z-50 px-8 bg-white">
                    <h1 class="pb-6 text-2xl font-bold">My Early Career</h1>
                    <p class="text-lg font-medium">Currently, my career focuses on marketing and product development. My experience analyzing consumer trends has given me a deeper insight into the motivations behind our purchasing habits. At the heart of it is the need to belong and to earn respect.</p>
                </div>
                <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
            </div>
        </div>
    </div>

    <div class="relative z-40 flex flex-col md:flex-row justify-center py-4 bg-[#F8F1E7]">
        <img class="-mb-32 mobile" src={boquet_up} alt="">
        <div class="flex items-center -mr-32 desktop max-w-80">
            <img src={boquet_left} alt="">
        </div>
        <div class="flex flex-col items-center justify-center max-w-xl">
            <img class="z-10 tear-north-sm" src={tear_south_sm_white} alt="">
            <div class="relative z-50 max-w-4xl px-8 bg-white">
                <h1 class="pb-6 text-2xl font-bold">Retail Therapy is for you</h1>
                <p class="text-lg font-medium">I created Retail Therapy because I want to inform people of these tendencies. We live in unpredictable economic times and as a member of Gen Z, the “buy everything, own nothing” generation, I know the allure of hyper-consumerism all too well. Despite what we like to believe, we are completely irrational beings. Being aware of it is the first step. I can help you there.</p>
            </div>
            <img class="z-10 tear-south-sm" src={tear_south_sm_white} alt="">
        </div>
        <div class="flex items-center -ml-32 desktop max-w-80">
            <img src={boquet_right} alt="">
        </div>
        <img class="-mt-32 mobile" src={boquet_down} alt="">
    </div>
    
    <img class="tear-south" src={tear_south_base_offwhite} alt="">
</section>

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

    @media(min-width: 425px) {
        .mobile {
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