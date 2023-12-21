<!-- HTML. -->
<main>
	<section id='get-in-touch'>
		<div class='flex-container'>
			<div class='get-in-touch-wrapper bold-title-letter-spacing'>
				<h1>GET IN</h1>
				<h1>TOUCH</h1>
			</div>
			<div class='socials-wrapper'>
				<div class='social'>
					<div class='icon'>
						<Icon icon='mdi:linkedin'/>
					</div>
					<div class='social-items'>
						<p>calvinconboy</p>
					</div>
				</div>
				<div class='social'>
					<div class='icon'>
						<Icon icon='clarity:email-line'/>
					</div>
					<div class='social-items'>
						<p>cconboy@umass.edu</p>
						<p>calvinconboy@gmail.com</p>
					</div>
				</div>
				<div class='social'>
					<div class='icon'>
						<Icon icon='ph:phone'/>
					</div>
					<div class='social-items'>
						<p>(978) 203-2296</p>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	.flex-container {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 1rem;
	}

	.get-in-touch-wrapper {
		width: 50%;
		text-align: right;
		font-size: 6rem;
	}

	.socials-wrapper {
		width: 50%;
	}

	.social {
		display: flex;
		align-items: center;
		gap: 0.5rem;
	}

	.icon {
		display: flex;
		font-size: 3.4rem;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	import Icon from '@iconify/svelte';
</script>