<!--This is a wrapper around all other content on your website. Things here
should be on every page, such as a header, footer, or the loading of global
styles.-->
<script>
	import '../app.css';
	import Footer from '$lib/components/Footer.svelte';
	import Header from '$lib/components/Header.svelte';
</script>

<div id="page-layout" class="flex flex-col min-h-screen">
	<Header />

	<!--This is the main content on every page-->
	<main class="flex-grow">
		<slot />
	</main>

	<Footer />
</div>