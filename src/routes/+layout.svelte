<script>
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	import './styles.css';
	let y = 0;
</script>

<svelte:head>
	<title>Dzaky Fattan's Portofolio</title>
	<meta name="description" content="Dzaky Fattan's Portofolio" />
</svelte:head>

<svelte:window bind:scrollY={y} />

<div class="app" on:scroll={(e) => y = window.scrollY}>
	<Header y = {y}/>

	<main class="flex flex-col flex-1 w-full box-border bg-black text-white">
		<slot />
	</main>

	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}
</style>
