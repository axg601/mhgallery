<script>
</script>

<svelte:head>
	<title>Gallery</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Gallery" />
</svelte:head>

<main>
	<section class="gallery" style="">
		<div class="item">
			Picture Slot
		</div>
		<div class="item">
			Picture Slot
		</div>
		<div class="item">
			Picture Slot
		</div>
		<div class="item">
			Picture Slot
		</div>
		<div class="item">
			Picture Slot
		</div>
		<div class="item">
			Picture Slot
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
	.item {
		background-color: gray;
		border: 1px solid black;
	}
	@media (max-width: 768px) {
		.gallery {
			grid-template-columns: 100%;
			padding-top: 1rem;
			width: 90%;
		}
	}
</style>
