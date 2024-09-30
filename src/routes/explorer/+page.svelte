<script>
// @ts-nocheck

    import View360, { EquirectProjection } from "@egjs/svelte-view360";
    import "@egjs/svelte-view360/css/view360.min.css";
    
    const imagePath = `${import.meta.env.BASE_URL}src/lib/images/pano.jpg`;

    const projection = new EquirectProjection({
      src: imagePath
    });
    </script>

<svelte:head>
	<title>Explorer</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Immersive Explorer" />
</svelte:head>

<main>
    <h2 class="bricolage-grotesque-medium">Check out the pavilion explorer below</h2>
	<section class="explorer" style="">
        <View360 class="is-16by9" projection={projection} gyro={true} autoplay={true} />
	</section>
    <p>This explorer was built using <a href="https://naver.github.io/egjs-view360/">View360</a>, a 360° panorama image / video viewer.</p>
</main>

<style>
.explorer {
    /* display: flex; */
    max-width: 66%;
    margin: auto;
    border: 1px solid black;
}
h2 {
    font-size: 2rem;
    text-align: center;
}
p {
    text-align: center;
    padding: 1rem;
}

@media (max-width: 768px) {
    .explorer {
        max-width: 90%;
    }
}

</style>
