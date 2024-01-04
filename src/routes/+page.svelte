<!-- Tab title. -->
<svelte:head>
	<title>Calvin Conboy | Portfolio</title>
</svelte:head>

<!-- HTML. -->
<main>
	<Hero></Hero>
	<SectionDivider></SectionDivider>
	<About></About>
	<SectionDivider></SectionDivider>
	<Contact></Contact>
	<Footer></Footer>
</main>

<!-- CSS. -->
<style></style>

<!-- TypeScript. -->
<script lang='ts'>
	import Hero from './hero.svelte';
	import About from './about.svelte';
	import Contact from './contact.svelte';
	import Footer from './footer.svelte';
	import SectionDivider from './section-divider.svelte';
</script>