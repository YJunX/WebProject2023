<script>
    import Navecation from '$lib/Navecation.svelte';
    import Footer from '$lib/footer.svelte'
    import '../main.css'

</script>

<section class="main">
	<Navecation/>
    <slot />
    <Footer/>
</section>
