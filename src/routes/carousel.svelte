<!-- HTML. -->
<main>
	<div class='carousel'>
		<!-- Second set of images needed for seamless loop. -->
		{#each {length: 2} as _}
			<div class='images'>
				<img src='./images/calvin-selfie.png' alt='Calvin Conboy Selfie' loading='lazy'>
				<img src='./images/calvin-forest.png' alt='Calvin Conboy Forest' loading='lazy'>
				<img src='./images/calvin-carhartt.png' alt='Calvin Conboy Carhartt' loading='lazy'>
				<img src='./images/calvin-pizza.png' alt='Calvin Conboy Pizza' loading='lazy'>
			</div>
		{/each}
	</div>
</main>

<!-- CSS. -->
<style>
	@keyframes slide {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-100%);
  }
}

.carousel {
	height: 32rem;
  overflow: hidden;
  position: relative;
	display: inline-flex;
}

.images {
	display: flex;
	height: 100%;
	animation: 20s slide linear infinite;
}

.images img {
  height: 100%;
}
</style>

<!-- TypeScript. -->
<script lang='ts'></script>