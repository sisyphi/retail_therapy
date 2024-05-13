<script>
    import tear_south_offwhite from '$lib/images/tear-south-offwhite.png';
</script>

<section>
    <img class="relative z-0 rotate-180 bg-transparent -mb-0.5 md:-mb-4 lg:-mb-6" src={tear_south_offwhite} alt="">
    <div class="relative z-10 bg-offwhite">
        <slot />
    </div>
    <img class="relative z-0 bg-transparent -mt-0.5 md:-mt-4 lg:-mt-6" src={tear_south_offwhite} alt="">
</section>