<script>
	import '../app.pcss';

    import Header from '$lib/components/Header.svelte';
    import Footer from '$lib/components/Footer.svelte';
</script>

<Header/>

<slot></slot>

<Footer />

<style>
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