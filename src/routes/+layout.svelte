<script>
	import '../app.pcss';
    import rt_logo from '../lib/images/rt-logo.svelte';
    import tear_south_base_offwhite from '$lib/images/tear-south-base-offwhite.png';
    
    let isMenuOpen = false;

    function toggleMenu() {
        isMenuOpen = !isMenuOpen;
    }
</script>

<header class="relative z-10 flex flex-col justify-center">
    <div class="z-50 flex justify-between px-4 pt-4 text-center mobile-header md:px-8 lg:px-20 xl:px-48 bg-[#F8F1E7]">
        <div class="flex mobile-logo-section">
            <a on:click={()=>(isMenuOpen = false)} href="/">
                <logo class="flex">
                    <svelte:component this={rt_logo} />
                </logo>
            </a>
        
            <button aria-controls="mobile-nav" aria-expanded="false" class="mobile-burger" on:click={toggleMenu}>
                <div class="burger-bar-1"/>
                <div class="burger-bar-2"/>
                <div class="burger-bar-3"/>
            </button>
        </div>

        <nav class:open={isMenuOpen} id="mobile-nav" class="flex text-xl mobile-nav">
            <ul class="flex items-center justify-center gap-8 mobile-nav-ul">
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option" href="/">
                    <li>home</li>
                </a>
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option" href="/articles/impulse_buy">
                    <li>articles</li>
                </a>
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option" href="/about">
                    <li>about me</li>
                </a>
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option md:bg-[#2A2A2A] md:text-white md:border-[0.5rem] md:border-[#2A2A2A]" href="/contact">
                    <li>contact me</li>
                </a>
            </ul>
        </nav>
    </div>
    <img class="tear-south" src={tear_south_base_offwhite} alt="">
</header>

<slot></slot>

<footer>
    <img class="tear-north" src={tear_south_base_offwhite} alt="">
    <div class="bg-[#F8F1E7]">
        
    </div>
</footer>

<style>
    /* header::after {
        content: "";
        position: absolute;
        top: 5.75rem;
        width: 100vw;
        height: 10rem;
        left: 0;
        background-size: 100%;
        background-repeat: no-repeat;
        background-image: url('../lib/images/rip-south.png');
        background: blue;
    } */

    :global(.tear-south) {
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

    :global(.tear-north) {
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

    /* Responsive Navbar */
    @media(max-width: 767px) {
        .mobile-header {
            display: flex;
            flex-direction: column;
            align-items: center;

            margin: 0;
            padding: 0;
        }

        .mobile-logo-section {
            display: flex;
            justify-content: space-between;
            align-items: center;

            width: 100%;

            margin-top: 1rem;
            padding: 0 1.5rem;
        }

        a {
            max-width: 12rem;
        }

        .mobile-burger {
            height: 2rem;
            aspect-ratio: 1;

            display: flex;
            align-items: center;
            justify-content: center;
        }

        .mobile-burger > div {
            height: 0.125rem;
            width: 1.5rem;
            background-color: #2A2A2A;

            position: absolute;
        }

        .burger-bar-1 {
            transform: translateY(-0.5rem);
        }

        .burger-bar-2 {
            transform: translateY(0px);
        }

        .burger-bar-3 {
            transform: translateY(0.5rem);
        }

        .mobile-nav {
            display: none;
        }

        .mobile-nav.open {
            display: block;
            width: 100%;
            
            margin: 0;
        }

        .mobile-nav-ul {
            display: flex;
            flex-direction: column;

            align-items: end;
            margin: 0.5rem 1.75rem 1.75rem 0;
        }

        .mobile-nav-option {
            display: flex;
            flex-direction: column;

            align-items: center;
        }
    }

    :global(logo > svg) {
        width: 12rem;
    }

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

    /* 
    :global(li) {
        font-size: 1.5rem;
        line-height: 1.75rem;
    }

    :global(img) {
        display: block;
        max-width: 100%;
    } */
</style>