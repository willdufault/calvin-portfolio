<!-- HTML. -->
<main>
	<div class='navigation-bar'>
		<a href='/' class='item item-fast'>Home</a>
		<a href='/professional-experience' class='item item-fast'>Professional Experience</a>
		<a href='/educational-experience' class='item item-smooth'>Educational Experience</a>
		<a href='/contact-me' class='item item-smooth'>Contact Me</a>
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
	}

	.item-fast:hover {
		text-decoration: underline;
	}

	.item-smooth {
		background: 
    linear-gradient(to right, black, black),
    linear-gradient(to right, white, white);
		background-size: 100% 0.1rem, 0 0.1rem;
		background-position: 100% 100%, 0 100%;
		background-repeat: no-repeat;
		transition: background-size 0.4s ease-out;
	}

	.item-smooth:hover {
		background-size: 0 0.1rem, 100% 0.1rem;
	}
</style>

<!-- TypeScript. -->
<script lang='ts'></script>