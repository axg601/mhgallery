<script>
	import logo from '$lib/images/sfu-logo.svg';
	import banner from '$lib/images/banner.jpg';
</script>

<header>
	<div class="navcontainer">
		<nav style="width: 60%; margin: auto">
			<div class="corner">
				<a href="https://www.francis.edu/">
					<img style="z-index: 50" src={logo} alt="SvelteKit" />
				</a>
			</div>
			<div style="padding-top: 2rem; width: 100%">
				<h1>
					Saint Francis University WRIT-102: Writing About Medicine
				</h1>
				<div style="display: flex; width: 100%; justify-content: end; font-size:large">
					<a href="/">
						Gallery
					</a>
					<a href="/about">
						About
					</a>
					<a href="https://www.francis.edu">
						SFU
					</a>
				</div>
			</div>
		</nav>
	</div>
	<section style="" class="container">
		<img src={banner} alt="Class visit on 9/20/24" class="banner" />
		<div class="overlay">
			<h1 class="overlaytext">Therapeutic Garden Support Project Gallery</h1>
			<h2 class="overlaytext">Fall 2024 WRIT-102: Writing About Medicine</h2>
		</div>
	</section>
</header>

<style>
	nav {
		padding: 0 8rem 0 8rem;
	}

	nav h1 {
		color: white;
		font-size: 1.25rem;
		text-align: right;
	}

	nav div a {
		color: white;
		font-size: 1rem;
		text-decoration: none;
		padding: 0 1rem;
	}
	h1 {
		font-size: 3.2rem;
	}
	h2 {
		font-size: 2rem;
	}

	.navcontainer {
		background-color: rgb(155, 11, 1);
		width: 100%; 
		display: flex; 
		justify-content: space-between; 
		margin: auto;
	}

	.container {
    	position: relative;
	}	
	.overlay {
		position: absolute;
		top: 25%;
		left: 10%;
		width: 100%;
	}

	.overlaytext {
		color: white;
		text-align: left;
		margin: 0%;
	}

	.banner {
		max-width: 100%;
		padding-bottom: 3rem;
		z-index: 0;
		position: relative;
	}

	.corner {
		width: 3em;
		height: 8.5em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 10em;
		height: 10em;
		transform: translateY(2rem);
		object-fit: contain;
	}

	nav {
		display: flex;
		justify-content: center;
	}

</style>
