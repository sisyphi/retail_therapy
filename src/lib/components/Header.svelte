<script>
    import tear_south_offwhite from '$lib/images/tear-south-offwhite.png';

    import Logo from '$lib/components/Logo.svelte';
    
    export let isMenuOpen = false;

    function toggleMenu() {
        isMenuOpen = !isMenuOpen;
    }
</script>

<header class="relative z-10 flex flex-col justify-center">
    <div class="z-50 flex justify-between px-4 pt-4 text-center mobile-header md:px-8 lg:px-20 xl:px-48 bg-offwhite">
        <div class="flex mobile-logo-section">
            <a on:click={()=>(isMenuOpen = false)} href="/">
                <logo class="flex">
                    <svelte:component this={Logo} />
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
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option" href="/articles">
                    <li>articles</li>
                </a>
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option" href="/about">
                    <li>about me</li>
                </a>
                <a on:click={()=>(isMenuOpen = false)} class="hover:underline mobile-nav-option md:bg-offblack md:text-white md:border-[0.5rem] md:border-offblack" href="/contact">
                    <li>contact me</li>
                </a>
            </ul>
        </nav>
    </div>
    <img class="relative z-0 transform bg-transparent -mt-0.5 md:-mt-4 lg:-mt-6" src={tear_south_offwhite} alt="">
</header>

<style>
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
</style>