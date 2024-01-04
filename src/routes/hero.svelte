<!-- HTML. -->
<main>
	<section class='hero'>
		<NavigationBar></NavigationBar>
		<div class='hero-body'>
			<div class='hero-body-left hide-overflow-x'>
				<div class='carousel-wrapper'>
					<Carousel></Carousel>
				</div>
			</div>
			<div class='hero-body-right'>
				<div class='text-wrapper'>
					<div class='title-wrapper bold-title-letter-spacing'>
						<h1>CALVIN</h1>
						<h1>CONBOY</h1>
					</div>
					<!-- <br/> -->
					<div class='description-wrapper'>
						<p>Marketing Major</p>
						<p>Economics Minor</p>
						<p>Candidate May 2024</p>
						<br/>
						<p>University of Massachusetts Amherst</p>
						<p>Isenberg School of Management</p>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	.carousel-wrapper {
		width: 70%;
	}

	.hide-overflow-x {
		overflow-x: hidden;
	}

	.title-wrapper {
		font-size: 8rem;
		width: fit-content;
		/* Divider. */
		border-bottom: 0.1rem solid white;
		padding-bottom: 1rem;
		margin-bottom: 1.5rem;
	}

	.description-wrapper p {
		font-size: 1.3rem;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	import NavigationBar from './navigation-bar.svelte';
	import Carousel from './carousel.svelte';
</script>