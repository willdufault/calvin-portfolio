<!-- HTML. -->
<main>
	<section id='hero'>
		<div class='flex-container'>
			<div class='isenberg'></div>
			<div class='text-wrapper'>
				<div class='name-wrapper bold-title-letter-spacing'>
					<h1>CALVIN</h1>
					<h1>CONBOY</h1>
				</div>
				<div class='degree-wrapper'>
					<p>Marketing Major</p>
					<p>Economics Minor</p>
					<p>Candidate May 2024</p>
				</div>
				<div class='amherst-wrapper'>
					<p>University of Massachusetts Amherst</p>
					<p>Isenberg School of Management</p>
				</div>
			</div>
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	section {
		margin: 4rem 4rem 8rem;
	}

	.flex-container {
		display: flex;
		gap: 1rem;
	}

	.isenberg {
		width: 50%;
		align-self: stretch;
		background: url('/images/isenberg.png');
		background-size: cover;
		background-repeat: no-repeat;
		background-position: right center;
		/* border: 2px solid red; */
	}

	.text-wrapper {
		width: 50%;
		display: flex;
		flex-direction: column;
		gap: 1.5rem;
		/* border: 2px solid blue; */
	}

	.name-wrapper {
		font-size: 9rem;
	}

	.degree-wrapper, .amherst-wrapper {
		font-size: 1.3rem;
	}

</style>

<!-- TypeScript. -->
<script lang='ts'></script>