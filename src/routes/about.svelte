<!-- HTML. -->
<main>
	<section>
		<div class='flex-container'>
			<div class='text-wrapper'>
				<h1 class='title'>About Me</h1>
				<div class='description-wrapper'>
					<p>
						My name is Calvin Conboy, and I am a current senior at the
						University of Massachusetts Amherst, within the Isenberg School of
						Business. I am a candidate for a BBA in marketing, along with a minor
						in economics.
					</p>
					<p>
						Growing up under a small business owner, I have learned the
						importance of hard work and the shown outcome that comes with
						dedication to every task I am working on. My passion for creativity
						shows through in every project I work on. With a strong belief in the
						power of effort-based outcomes, I strive to bring a unique and
						innovative approach to every project I'm assigned. My
						creativity-forward work approach has not only helped me in my past
						professional experience, but also in the success when leading projects
						within educational settings. 
					</p>
					<p>
						My passions outside of professional settings include attending live
						events, following the NBA, and spending time outside.
					</p>
				</div>
			</div>
			<div class='carousel-wrapper hide-overflow-x'>
				<Carousel></Carousel>
			</div>
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	.text-wrapper {
		text-align: center;
		width: 50%;
	}

	.description-wrapper {
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}

	.carousel-wrapper {
		width: 50%;
	}

	.hide-overflow-x {
		overflow-x: hidden;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	import Carousel from './carousel.svelte';
</script>