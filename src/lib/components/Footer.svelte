<script>
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';
    import tear_south_offwhite from '$lib/images/tear-south-offwhite.png';

    import Logo from '$lib/components/Logo.svelte';

    let isMenuOpen = false;
</script>

<footer>
    <img class="relative z-0 transform bg-transparent rotate-180 -mb-0.5 md:-mb-4 lg:-mb-6" src={tear_south_offwhite} alt="">
    <div class="relative z-10 flex flex-col justify-center px-8 pb-4 sm:flex-row sm:justify-between md:px-8 lg:px-20 xl:px-48 bg-[#F8F1E7]">
        <div class="my-4">
            <div class="flex justify-center pb-4 sm:justify-normal">
                <a href="/">
                    <logo class="flex">
                        <svelte:component this={Logo} />
                    </logo>
                </a>
            </div>
            <div class="flex justify-center pb-4 sm:justify-normal">
                <a class="text-sm hover:underline" href="mailto:maria.ysabel.dinsay@gmail.com">maria.ysabel.dinsay@gmail.com</a>
            </div>
            <div class="flex justify-center sm:justify-normal">
                <a class="mx-2 size-6" href="https://www.linkedin.com/in/ysabel-dinsay/"><img src={linkedin_icon_graphic} alt="Linkedin logo"></a>
                <a class="mx-2 size-6" href="https://www.instagram.com/ysabeldinsay/"><img src={ig_icon_graphic} alt="Instagram logo"></a>
            </div>
        </div>
        <div class="my-4">
            <nav class="">
                <p class="mb-2 text-lg text-center sm:text-left">PAGES</p>
                <ul class="text-center sm:text-left">
                    <a class="hover:underline" href="/">
                        <li class="mb-2">home</li>
                    </a>
                    <a class="hover:underline" href="/articles">
                        <li class="mb-2">articles</li>
                    </a>
                    <a class="hover:underline" href="/about">
                        <li class="mb-2">about me</li>
                    </a>
                    <a class="hover:underline" href="/contact">
                        <li class="mb-2">contact me</li>
                    </a>
                </ul>
            </nav>
        </div>
    </div>
</footer>