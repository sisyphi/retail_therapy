<script>
	import '../app.pcss';
    import ig_icon_graphic from '$lib/images/ig-icon-graphic.png';
    import linkedin_icon_graphic from '$lib/images/linkedin-icon-graphic.png';

    import Header from '$lib/components/Header.svelte';
    import Footer from '$lib/components/Footer.svelte';
</script>

<Header />

<slot></slot>

<Footer />

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