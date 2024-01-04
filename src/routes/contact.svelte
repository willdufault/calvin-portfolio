<!-- HTML. -->
<main>
	<section>
		<div class='flex-container'>
			<div class='title-wrapper bold-title-letter-spacing'>
				<h1>GET IN</h1>
				<h1>TOUCH</h1>
			</div>
			<div class='socials-wrapper'>
				<a class='social' href='https://linkedin.com/in/calvinconboy' target='_blank'>
					<div class='icon'>
						<Icon icon='mdi:linkedin'/>
					</div>
					<div class='social-items'>
						<p>calvinconboy</p>
					</div>
				</a>
				<a class='social' href='mailto:calvinconboy@gmail.com' target='_blank'>
					<div class='icon'>
						<Icon icon='clarity:email-line'/>
					</div>
					<div class='social-items'>
						<p>calvinconboy@gmail.com</p>
					</div>
				</a>
				<a href='javascript:;' class='social' on:click={() => copyPhoneNumber()}>
					<div class='icon'>
						<Icon icon='ph:phone'/>
					</div>
					<div class='social-items'>
						<p>{phone_number}</p>
					</div>
				</a>
			</div>
		</div>
	</section>
</main>

<!-- CSS. -->
<style>
	.title-wrapper {
		width: 50%;
		text-align: right;
		font-size: 6rem;
	}

	.socials-wrapper {
		width: 50%;
	}

	.social {
		width: fit-content;
		display: flex;
		align-items: center;
		gap: 0.5rem;
		color: white;
		text-decoration: none;
	}

	.icon {
		display: flex;
		font-size: 3.4rem;
	}

	.social-items p {
		color: white;
		text-decoration: none;
	}
	.social:hover .icon, .social:hover p {
		color: var(--highlight-blue);
	}
</style>

<!-- TypeScript. -->
<script lang='ts'>
	import Icon from '@iconify/svelte';

	// Calvin Conboy's phone number.
	let phone_number: string = '(339) 203-2296'; 

	/*
	Copy Calvin's phone number to the clipboard and alert the user.
	*/
	function copyPhoneNumber(): void {
		// Try to write to the clipboard.
		navigator.clipboard.writeText(phone_number)
		.then(() => {
			// Copy the phone number to clipboard.
			navigator.clipboard.writeText(phone_number);

			// Alert the user.
			alert('Phone number copied to clipboard.');
		})
		.catch((error) => {
			// Print the error to console.
			console.error('Failed to copy: ', error);
		});
	}
</script>