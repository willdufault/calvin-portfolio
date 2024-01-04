<!-- HTML. -->
<main>
	<div class='navigation-bar'>
		<a href='' on:click={() => openPage('home')} class='item'>Home</a>
		<a href='' on:click={() => openPage('professional-experience')} class='item'>Professional Experience</a>
		<a href='' on:click={() => openPage('educational-experience')} class='item'>Educational Experience</a>
		<a href='' on:click={() => openPage('contact-me')} class='item'>Contact Me</a>
	</div>
</main>

<!-- CSS. -->
<style>
	.navigation-bar {
		display: flex;
		justify-content: center;
		gap: 10%;
		margin-top: 2rem;
	}

	.item {
		color: white;
		text-decoration: none;
		/* Make the text look like it is above the underline. */
		text-shadow: -1px 0 black, 1px 0 black, -2px 0 black, 2px 0 black;
		background: linear-gradient(to right, black, black), linear-gradient(to right, white, white);
		background-size: 100% 0.1rem, 0 0.1rem;
		background-position: 100% 100%, 0 100%;
		background-repeat: no-repeat;
		transition: background-size 0.4s ease-out;
	}

	.item:hover {
		background-size: 0 0.1rem, 100% 0.1rem;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	import { base } from '$app/paths';

	/*
	Add the base URL to the beginning of the path.
	*/
	function openPage(page: string): void {
		// Home page is the base URL.
		if(page === 'home') {
			page = '';
		}

		// Open the page in the current tab.
		window.open(`${base}/${page}`, '_self');
	}
</script>