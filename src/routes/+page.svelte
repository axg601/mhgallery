<script>
	import sstophel from '$lib/images/sstophel.jpeg';
	import mluger from '$lib/images/mluger.jpeg';
	import hmeyers from '$lib/images/hmyers.png';
	import awells from '$lib/images/awells.jpeg';
	import mgolden from '$lib/images/mgolden.jpg';
	import oclark from '$lib/images/oclark.jpg';
	import jcariaso from '$lib/images/jcariaso.jpeg';
	import aprince from '$lib/images/aprince.jpg';
</script>

<svelte:head>
	<title>Gallery</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Gallery" />
</svelte:head>

<main>
	<section class="gallery" style="">
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={sstophel} alt="" class="item">
			<p>Sophie Stophel and Sierra Crum making suncatchers.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={mluger} alt="" class="item">
			<p>Austin Bender and Mali Luger's gnome garden.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small landscape" style="">
			<img src={hmeyers} alt="" class="item">
			<p>Hunter Myers and Caden Schenk's bench.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={awells} alt="" class="item">
			<p>Aubrie Wells and Olivia Clark's sea urchin shell medusae.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={oclark} alt="" class="item">
			<p>Aubrie Wells and Olivia Clark's medusae hung in the pavilion.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={mgolden} alt="" class="item">
			<p>Alyssa Giovinazzo and Mary Golden's painted pots.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small">
			<img src={jcariaso} alt="" class="item">
			<p>Joaquim Cariaso's decorated gourds.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small landscape" style="">
			<img src={aprince} alt="" class="item">
			<p>Alyssa Irwin and Ava Prince's re-stained Veg Trug #2.</p>
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
	.landscape {
		grid-column: span 2;
	}
	@media (max-width: 768px) {
		.gallery {
			grid-template-columns: 100%;
			padding-top: 1rem;
			width: 90%;
		}
		.landscape {
			grid-column: span 1;
		}
	}
</style>
