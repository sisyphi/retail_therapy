<script>
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';
    import tear_south_offwhite from '$lib/images/tear-south-offwhite.png';

    import Logo from '$lib/components/Logo.svelte';

    export const prerender = true
</script>

<footer>
    <img class="relative z-0 transform bg-transparent rotate-180 -mb-0.5 md:-mb-4 lg:-mb-6" src={tear_south_offwhite} alt="">
    <div class="relative z-10 flex flex-col justify-center px-8 pb-4 md:flex-row md:justify-between md:px-8 lg:px-20 xl:px-48 bg-offwhite">
        <div class="my-4">
            <div class="flex justify-center pb-4 md:justify-normal">
                <a href="/">
                    <logo class="flex">
                        <svelte:component this={Logo} />
                    </logo>
                </a>
            </div>
            <div class="flex justify-center pb-4 md:justify-normal">
                <a class="hover:underline" href="mailto:maria.ysabel.dinsay@gmail.com">maria.ysabel.dinsay@gmail.com</a>
            </div>
            <div class="flex justify-center gap-4 md:justify-normal">
                <a class="size-6" href="https://www.linkedin.com/in/ysabel-dinsay/"><img src={linkedin_icon_graphic} alt="Linkedin logo"></a>
                <a class="size-6" href="https://www.instagram.com/ysabeldinsay/"><img src={ig_icon_graphic} alt="Instagram logo"></a>
            </div>
        </div>
        <div class="mx-8 my-4">
            <nav class="">
                <p class="mb-2 font-serif text-lg font-semibold text-center md:text-left">pages</p>
                <ul class="text-center md:text-left">
                    <a class="hover:underline" href="/">
                        <li class="mb-2 font-sans font-medium">home</li>
                    </a>
                    <a class="hover:underline" href="/articles">
                        <li class="mb-2 font-sans font-medium">articles</li>
                    </a>
                    <a class="hover:underline" href="/about">
                        <li class="mb-2 font-sans font-medium">about me</li>
                    </a>
                    <a class="hover:underline" href="/contact">
                        <li class="mb-2 font-sans font-medium">contact me</li>
                    </a>
                </ul>
            </nav>
        </div>
        <div class="mx-auto my-4 md:mx-0 max-w-64">
            <form action="/contact" netlify name="netlify-email-sub-form" method="POST" data-netlify="true">
            <!-- <form action="/contact" name="netlify-email-sub-form" method="POST" netlify-honeypot="bot-field" data-netlify="true"> -->
                <div class="flex flex-col gap-2">
                    <input type="hidden" name="form-name" value="netlify-email-sub-form" />
                    <label class="w-full">
                        <p class="font-serif text-lg font-semibold">subscribe for updates</p>
                        <input class="w-full p-2 font-sans placeholder:italic font-light bg-transparent placeholder:text-offblack placeholder:opacity-50 border-offblack border-b-[1px]" type="email" name="email" placeholder="your email here"/>
                    </label>
                    <input type="submit" class="px-4 py-1 my-2 ml-auto font-serif font-semibold text-white text-md hover:underline mobile-nav-option bg-offblack border-offblack" value="submit"/>
                    <p class="font-sans text-xs leading-4 text-justify font-extralight">by submitting your email, this means you have read and agree to the <a class="font-sans italic underline font-extralight" href="/privacy-policy">Privacy Policy</a></p>
                </div>
            </form>
        </div>
    </div>
</footer>