<script>
    import tear_south_base_offwhite from '$lib/images/tear-south-base-offwhite.png';
    import tear_south_sm_white from '$lib/images/tear-south-sm-white.png';
    import tear_south_sm_offwhite from '$lib/images/tear-south-sm-offwhite.png';
</script>

<section>
    <img class="relative z-0 transform rotate-180 bg-transparent -mb-0.5 md:-mb-4 lg:-mb-6" src={tear_south_base_offwhite} alt="">
    <div class="relative z-10 bg-[#F8F1E7]">
        <slot />
    </div>
    <img class="relative z-0 transform bg-transparent -mt-0.5 md:-mt-4 lg:-mt-6" src={tear_south_base_offwhite} alt="">
</section>