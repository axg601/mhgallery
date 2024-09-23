<script>
</script>

<svelte:head>
	<title>Gallery</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Gallery" />
</svelte:head>

<main>
	<section class="gallery" style="width: 66%; margin: auto;">
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
	}
	.item {
		background-color: gray;
		border: 1px solid black;
	}
</style>
