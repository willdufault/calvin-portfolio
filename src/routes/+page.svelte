<!-- Set tab icon and title. -->
<svelte:head>
	<link rel='icon' href='favicon.png' />
	<title>Calvin Conboy | Portfolio</title>
</svelte:head>

<!-- HTML. -->
<main>
	<Hero></Hero>
	<About></About>
	<WorkExperience></WorkExperience>
	<EducationalExperience></EducationalExperience>
	<Contact></Contact>
</main>

<!-- CSS. -->
<style></style>

<!-- TypeScript. -->
<script lang='ts'>
	import Hero from './hero.svelte';
	import About from './about.svelte';
	import WorkExperience from './work-experience.svelte';
	import EducationalExperience from './educational-experience.svelte';
	import Contact from './contact.svelte';
</script>