<script>
</script>

<svelte:head>
	<title>Gallery</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Gallery" />
</svelte:head>

<main>
	<section class="gallery" style="width: 66%; margin: auto;">
		<div class="item">
			content
		</div>
		<div class="item">
			content
		</div>
		<div class="item">
			content
		</div>
		<div class="item">
			content
		</div>
		<div class="item">
			content
		</div>
		<div class="item">
			content
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
		background-color: green;
		border: 1px solid black;
	}
</style>
