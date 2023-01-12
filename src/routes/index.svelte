<script>
    import Header from "$lib/components/Header.svelte"
    import Hero from "$lib/components/Hero.svelte"
	import Main from '$lib/components/Main.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>
<div class="Index">
    <Header />
    <div class="Index--container">
        <Hero />
    </div>
    <div class="Container-main">
        <Main/>
        <Footer />
    </div>
</div>
<style>
    .Index{
        background-color: #0f0f0f;
    }
    .Index--container{
        width: 90%;
        max-width: 1280px;
        margin: 0 auto;
    }
    .Container-main{
        width: 90%;
        margin: 0 auto;
    }
    @media screen and (min-width: 768px) {
        .Container-main{
            width: 85%;
            margin: 0 auto;
            max-width: 1440px;
        }
    }
</style>