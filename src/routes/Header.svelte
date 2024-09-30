<script>
	import logo from '$lib/images/sfu-logo.svg';
	import banner from '$lib/images/banner.jpg';
</script>

<header>
	<div class="navcontainer">
		<nav>
			<div class="corner">
				<a href="/">
					<img style="z-index: 50" src={logo} alt="SvelteKit" />
				</a>
			</div>
			<div class="navcontent">
				<h1 class="bricolage-grotesque-large">
					Saint Francis University WRIT-102: Writing About Medicine
				</h1>
				<div class="links">
					<a href="/">
						Gallery
					</a>
					<a href="/explorer">
						Explorer
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
			<h1 class="overlaytextlg bricolage-grotesque-large">Therapeutic Garden Support Project</h1>
			<h2 class="overlaytextsm ">Fall 2024 WRIT-102: Writing About Medicine</h2>
		</div>
	</section>
</header>

<style>
	nav {
		width: 100%; 
		margin: auto;
		display: flex;
		justify-content: space-evenly;
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
		margin: auto;
	}
	.container {
    	position: relative;
	}	
	.overlay {
		position: absolute;
		top: 25%;
		left: 10%;
		width: 50vw;
	}
	.overlaytextlg{
		color: white;
		text-align: left;
		margin: 0%;
		width: 50vw;
	}

	.overlaytextsm {
		color: white;
		text-align: left;
		margin: 0%;
		width: 50vw;
	}

	.banner {
		max-width: 100%;
		padding-bottom: 3rem;
		z-index: 0;
		position: relative;
	}
	.navcontent {
		padding-top: 2rem;
	}
	.links {
		display: flex; 
		width: 100%; 
		justify-content: end; 
		font-size: large;
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
    @media (max-width: 768px) {
        nav {
            padding: 0;
			margin: 0;
			display: block;
			width: 100%;
        }	
		nav h1 {
			text-align: center;
		}
		.navcontent {
			padding-top: 0;
			padding: 1rem;
		}
        .corner {
			display: none;
        }
		.links {
			justify-content: center;
		}
		.banner {
			display: none;
		}
		.overlay {
			position: static;
			width: 100vw;
		}
		.overlay .overlaytextlg {
			margin: 0;
			padding: 0;
			width: 100vw;
			text-align: center;
			color: black;
		}
		.overlaytextlg {
			font-size: 1rem;
			text-align: center;
			width: 100%;
		}
		.overlaytextsm {
			display: none;
		}
    }
</style>
