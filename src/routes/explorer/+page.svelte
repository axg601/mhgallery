<script>
// @ts-nocheck

    import View360, { EquirectProjection } from "@egjs/svelte-view360";
    import "@egjs/svelte-view360/css/view360.min.css";
    import corner from '$lib/images/corner.jpg';
    import door from '$lib/images/door.jpg';
    import parking from '$lib/images/parking.jpg';
    import pavilion from '$lib/images/pavilion.jpg';

    const cornerProjection = new EquirectProjection({
        src: corner
    });
    const doorProjection = new EquirectProjection({
        src: door
    });
    const parkingProjection = new EquirectProjection({
        src: parking
    });
    const pavilionProjection = new EquirectProjection({
        src: pavilion
    });
</script>

<svelte:head>
	<title>Explorer</title>
	<meta name="description" content="SFU WRIT-102 Botany Project Immersive Explorer" />
</svelte:head>

<main>
    <h2 class="bricolage-grotesque-medium">Check out the pavilion explorer below</h2>
    <p>Click and drag to explore the 360° panorama image.</p>
        <section class="explorer" style="">
            <View360 class="is-16by9" projection={parkingProjection} gyro={true} autoplay={false}  />
        </section>
        <section class="explorer" style="">
            <View360 class="is-16by9" projection={cornerProjection} gyro={true} autoplay={false}  />
        </section>
        <section class="explorer" style="">
            <View360 class="is-16by9" projection={pavilionProjection} gyro={true} autoplay={true}  />
        </section>
    <p>This explorer was built using <a href="https://naver.github.io/egjs-view360/">View360</a>, a 360° panorama image / video viewer.</p>
</main>

<style>
.explorer {
    width: 66%;
    margin: auto;
    border: 1px solid black;
    margin-bottom: 2rem;
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
        width: 90%;
        margin: none;
    }
}

</style>
