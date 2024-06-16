<script lang="ts">
	import { onMount } from 'svelte';
	import { page } from '$app/stores';
	import { derived } from 'svelte/store';
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';

	const title = derived(page, ($page) => $page.data.title || 'Default Title');

	let pageTitle = 'Default Title';

	title.subscribe((value) => {
		pageTitle = value;
	});

	onMount(() => {
		document.title = pageTitle;
	});
</script>

<Navbar />
<main>
	<slot />
</main>
<Footer />
