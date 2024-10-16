<script>
	import sstophel from '$lib/images/sstophel.jpeg';
</script>

<svelte:head>
	<title>Gallery</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Gallery" />
</svelte:head>

<main>
	<section class="gallery" style="">
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={sstophel} alt="Sophie Stophel and Sierra Crum" class="item">
			<p>Sophie Stophel and Sierra Crum making suncatchers.</p>
		</div>
	</section>
</main>

<style>
	.gallery {
		display: grid;
		grid-template-columns: 50% 50%;
		gap: 1rem;
		width: 66%; 
		margin: auto;
	}
	.itemcontainer {
		width: 100%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		font-size: 1.2rem;
	}
	.item {
		border-radius: 1rem;
		width: 100%;
	}
	@media (max-width: 768px) {
		.gallery {
			grid-template-columns: 100%;
			padding-top: 1rem;
			width: 90%;
		}
	}
</style>
