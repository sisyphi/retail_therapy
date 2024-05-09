<script>
    import tear_south_base_offwhite from '$lib/images/tear-south-base-offwhite.png';
    import tear_south_sm_white from '$lib/images/tear-south-sm-white.png';
    import tear_south_sm_offwhite from '$lib/images/tear-south-sm-offwhite.png';
</script>

<section>
    <img class="transform rotate-180 bg-transparent -mb-0.5 md:-mb-4 lg:-mb-6" src={tear_south_base_offwhite} alt="">
    <img class="tear-north" src={tear_south_base_offwhite} alt="">
    <div class="bg-[#F8F1E7]">
        <slot />
    </div>
    <img class="transform bg-transparent -mt-0.5 md:-mt-4 lg:-mt-6" src={tear_south_base_offwhite} alt="">
    <img class="tear-south" src={tear_south_base_offwhite} alt="">
</section>

<style>
    .tear-south {
        background-color: transparent;
        /* filter: drop-shadow(0 0.3rem 0.6rem black); */

        margin-top: -0.1rem;

        @media(min-width: 768px) {
            margin-top: -1rem;
        }

        @media(min-width: 1024px) {
            margin-top: -1.5rem;
        }
    }

    .tear-north {
        transform: rotate(180deg);

        background-color: transparent;
        /* filter: drop-shadow(0 -0.3rem 0.6rem black); */

        margin-bottom: -0.1rem;

        @media(min-width: 768px) {
            margin-bottom: -1rem;
        }

        @media(min-width: 1024px) {
            margin-bottom: -1.5rem;
        }
    }
</style>
