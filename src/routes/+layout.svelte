<script>
	import '../app.pcss';
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';

    import Header from '$lib/components/Header.svelte';
</script>

<Header />

<slot></slot>

<footer>
    <!-- <img class="relative z-0 tear-north" src={tear_south_base_offwhite} alt="">
    <div class="relative z-50 bg-[#F8F1E7]">
        <div class="">
            <div class="">
                <div>
                    <a on:click={()=>(isMenuOpen = false)} href="/">
                        <logo class="flex">
                            <svelte:component this={rt_logo} />
                        </logo>
                    </a>
                </div>
                <div>
                    <a class="text-sm text-center hover:underline" href="mailto:maria.ysabel.dinsay@gmail.com">maria.ysabel.dinsay@gmail.com</a>
                </div>
                <div class="flex">
                    <a class="size-6" href="https://www.linkedin.com/in/ysabel-dinsay/"><img src={linkedin_icon_graphic} alt="Linkedin logo"></a>
                    <a class="size-6" href="https://www.instagram.com/ysabeldinsay/"><img src={ig_icon_graphic} alt="Instagram logo"></a>
                </div>
            </div>
        </div>
    </div> -->
</footer>

<style>
	:global(body) {
		background-color: #2A2A2A;	
        color: #2A2A2A;
  	}

    :global(.literata-bold) {
        font-family: "Literata", serif;
        font-optical-sizing: auto;
        font-weight: 700;
        font-style: normal;
    }

    :global(.general-sans-medium) {
        font-family: "General Sans", serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
    }


    :global(body, p) {
        font-family: "General Sans", serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
        /* font-size: 1rem; */
        /* line-height: 1.5rem; */
    }

    :global(h1, a) {
        font-family: "Literata", serif;
        font-optical-sizing: auto;
        font-weight: 700;
        font-style: normal;
        /* font-size: 2rem; */
        /* line-height: 3rem; */
    }
</style>