<script>
    import Navecation from '$lib/Navecation.svelte';
    import Footer from '$lib/footer.svelte'

</script>

<section class="main">
	<Navecation/>
    <slot />
    <Footer/>
</section>
