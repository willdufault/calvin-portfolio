<!-- HTML. -->
<main>
	<section>
		<div class='jobs-wrapper'>
			{#each experiences as experience, index}
				<div class={'job' + (index % 2 == 1 ? ' job-reverse' : '')}>
					<img class='logo' src={experience.image_url} alt={experience.image_alt} loading='lazy'>
					<p class='description'>{experience.description}</p>
				</div>
			{/each}
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	section {
		text-align: center;
	}

	.jobs-wrapper {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 6rem;
	}

	.job {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 2rem;
	}

	.job-reverse {
		flex-direction: row-reverse;
	}

	.logo {
		max-height: 14rem;
		max-width: 28rem;
	}

	.description {
		font-size: 1.1rem;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	// Professional Experience information.
	interface ExperienceData {
		company: string,
		description: string,
		image_url: string,
		image_alt: string
	}

	// List of professional experiences.
	let experiences: ExperienceData[] = [
		{
			company: 'Karma Coffee',
			description: 'I started working at Karma Coffee when I was only 13 years old, working the \
			register and helping with small wholesale orders. I quickly grew within the company, working \
			within every part of the business. Daily tasks ranging from cleaning the 1940\'s Probat \
			roaster, to communicating directly with wholesale accounts such as Whole Foods, and \
			restaurants across Eastern Massachusetts. Working at a small business taught me a wide variety \
			of skills that involved every aspect of a company. Recently, I have worked as the head of \
			hiring for the company, creating and maintaining job postings for all positions for the \
			business.',
			image_url: './images/karma-coffee-logo.jpg',
			image_alt: 'Karma Coffee Logo',
		},
		{
			company: 'Aflac',
			description: 'During my work with Aflac as a benefits advisor intern, I conducted business to \
			business sales through phone, and in-person meetings with local businesses throughout eastern \
			Massachusetts, Connecting with over 25 businesses daily. Along with sales, I studies market \
			trends to identify optimal marketing tactics for small businesses.',
			image_url: './images/aflac-logo.jpg',
			image_alt: 'Aflac Logo',
		},
		{
			company: 'Different Leaf',
			description: 'Different Leaf Magazine is a "Journal of Cannabis Culture". As an intern, I \
			completed a variety of different tasks across all areas of the publishing process. I worked \
			directly alongside the head publisher to find high-end cannabis companies to partner with on a \
			nationwide setting. Along with performing research, I worked alongside a freelance creative \
			team for a successful rollout for the apparel company, "Boast". The campaign is set to release \
			in January of 2024 as a re-release of a 70\'s tennis and squash apparel line that utilized the \
			Japanese maple leaf as it\'s logo. My work was used in both the Fall and Summer 2023 \
			publications.',
			image_url: './images/different-leaf-logo.jpg',
			image_alt: 'Different Leaf Logo',
			
		}
	];
</script>