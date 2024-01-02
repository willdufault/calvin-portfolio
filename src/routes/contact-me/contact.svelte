<!-- HTML. -->
<main>
	<section class='hero'>
		<NavigationBar></NavigationBar>
		<div class='hero-body'>
			<div class='hero-body-left'>
				<div class='title-wrapper bold-title-letter-spacing'>
					<h1>GET IN</h1>
					<h1>TOUCH</h1>
				</div>
			</div>
			<div class='hero-body-right'>
				<div class='socials-wrapper'>
					<div class='social'>
						<div class='icon'>
							<Icon icon='mdi:linkedin'/>
						</div>
						<div class='social-items'>
							<a href='https://linkedin.com/in/calvinconboy'>calvinconboy</a>
						</div>
					</div>
					<div class='social'>
						<div class='icon'>
							<Icon icon='clarity:email-line'/>
						</div>
						<div class='social-items'>
							<a href='mailto:calvinconboy@gmail.com'>calvinconboy@gmail.com</a>
							<br/>
							<a href='mailto:cconboy@umass.edu'>cconboy@umass.edu</a>
						</div>
					</div>
					<div class='social'>
						<div class='icon'>
							<Icon icon='ph:phone'/>
						</div>
						<div class='social-items'>
							<a href='' on:click={() => copyPhoneNumber()}>{phone_number}</a>
						</div>
					</div>
				</div>
			</div>
			
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	.title-wrapper {
		font-size: 8rem;
	}

	.social {
		width: fit-content;
		display: flex;
		align-items: center;
		gap: 0.5rem;
	}

	.icon {
		display: flex;
		font-size: 4.5rem;
	}

	.social-items a {
		font-size: 1.3rem;
		color: white;
		text-decoration: none;
	}
	.social:hover .icon, .social:hover .social-items a {
		color: #5ab8ff;
	}

</style>

<!-- TypeScript. -->
<script lang='ts'>
	import NavigationBar from '../navigation-bar.svelte';
	import Icon from '@iconify/svelte';

	let phone_number: string = '(339) 203-2296'; 

	function copyPhoneNumber(): void {
		// Copy the phone number to clipboard.
		navigator.clipboard.writeText(phone_number);

		// Alert the user.
		alert('Phone number copied to clipboard.');
	}
</script>