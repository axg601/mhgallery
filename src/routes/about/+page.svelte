<script>
// @ts-nocheck

	import View360, { EquirectProjection } from "@egjs/svelte-view360";
    import "@egjs/svelte-view360/css/view360.min.css";
    import panoImage from '$lib/images/class.jpg';

	const projection = new EquirectProjection({
		src: panoImage 
	});
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<main>
	<div class="text-column">
		<h1 class="bricolage-grotesque-large">About this site</h1>
		<p>
			This site is a showcase of student work from WRIT-102: Writing About Medicine at Saint Francis University in Loretto, PA. The work was done to increase the livelihood of the elderly living at the Cambria Care Facility in Ebensburg, PA through botanical means. 
			This center is a nursing home operating with 226 residents and 301 certified beds and specializes in caring senior citizens and making their life happier. This facility has been certified to participate in Medicare and Medicaid programs since April 27, 1990.
		</p>
		<p>
			We believe that this initiative, taken by our professor Dr. Timothy Bintrim, will alleviate the stress and worries people living here experience and will have a lasting impact not only on those working and residing in Cambria Care, but also on the students at Saint Francis University. Our classmates have put in a ton of effort in making and doing work that will help the residents and make them smile looking at what we've done. Further, this website is a means to allow friends and family to draw closer to the elders in care at the nursing home and as an acknowledgment to our school's love for the elderly. We are grateful for the opportunity to make an impact from simple text on a server.
		</p>
		<p>				
			This is a <a href="https://kit.svelte.dev">SvelteKit</a> app. You can make your own by typing the
			following into your command line, with node package manager installed, and following the prompts:
		</p>
		<pre>npm create svelte@latest</pre>
	</div>
	<section class="explorer" style="">
		<View360 
			class="is-16by9" 
			projection={projection} 
			gyro={true} 
			autoplay={false} 
			initialPitch={20}
			initialYaw={10}
		/>
	</section>
</main>


<style>
	.explorer {
		display: block;
		max-width: 33%;
		margin: auto;
		border: 1px solid black;
	}
	div {
		padding: 1rem;
	}
	@media (max-width: 768px) {
    .explorer {
        width: 90%;
		max-width: none;
    }
}
</style>