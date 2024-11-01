<script>
	import sstophel from '$lib/images/sstophel.jpeg';
	import mluger from '$lib/images/mluger.jpeg';
	import hmeyers from '$lib/images/hmyers.png';
	import awells from '$lib/images/awells.jpeg';
	import mgolden from '$lib/images/mgolden.jpg';
	import oclark from '$lib/images/oclark.jpg';
	import jcariaso from '$lib/images/jcariaso.jpeg';
	import aprince from '$lib/images/aprince.jpg';
	import bintrim1 from '$lib/images/bintrim1.jpg';
	import bintrim2 from '$lib/images/bintrim2.jpg';
	import bintrim3 from '$lib/images/bintrim3.jpg';
	import bintrim4 from '$lib/images/bintrim4.jpg';
	import bintrim5 from '$lib/images/bintrim5.jpg';
	import bintrim6 from '$lib/images/bintrim6.jpg';
	import bintrim7 from '$lib/images/bintrim7.jpg';
	import bintrim8 from '$lib/images/bintrim8.jpg';
	import bintrim9 from '$lib/images/bintrim9.jpg';
	import bintrim10 from '$lib/images/bintrim10.jpg';
	import bintrim11 from '$lib/images/bintrim11.jpg';
	import bintrim12 from '$lib/images/bintrim12.jpg';
	import bintrim13 from '$lib/images/bintrim13.jpg';
	import bintrim14 from '$lib/images/bintrim14.jpg';
	import bintrim15 from '$lib/images/bintrim15.jpg';
	import bintrim16 from '$lib/images/bintrim16.jpg';
	import bintrim17 from '$lib/images/bintrim17.jpg';
	import bintrim18 from '$lib/images/bintrim18.jpg';
	import bintrim19 from '$lib/images/bintrim19.jpg';
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
			<p>Austin Bender and Mali Luger's potted fairy garden.</p>
		</div>
		<div class="itemcontainer bricolage-grotesque-small landscape" style="">
			<img src={hmeyers} alt="" class="item">
			<p>Hunter Myers and Caden Schenk's inscribed bench.</p>
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
		<div class="itemcontainer" style="">
			<img src={bintrim1} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim5} alt="" class="item">
		</div>
		<div class="itemcontainer landscape" style="">
			<img src={bintrim2} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim3} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim4} alt="" class="item">
		</div>
		<div class="itemcontainer landscape" style="">
			<img src={bintrim6} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim7} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim8} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim9} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim10} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim11} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim16} alt="" class="item">
		</div>
		<div class="itemcontainer landscape" style="">
			<img src={bintrim12} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim13} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim14} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim17} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim18} alt="" class="item">
		</div>
		<div class="itemcontainer landscape" style="">
			<img src={bintrim19} alt="" class="item">
		</div>
		<div class="itemcontainer" style="">
			<img src={bintrim15} alt="" class="item">
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
