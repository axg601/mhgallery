<script>
	import Header from './Header.svelte';
	import linkedIn from '$lib/images/linkedin.png'
	import '../app.css';
</script>

<div class="app">
	<Header />
	<main>
		<slot />
	</main>

	<footer>
		<p>Built by Ashton George <a href="https://www.linkedin.com/in/ashton-george-160619240/"><img class="social" src={linkedIn} alt="LinkedIn"/></a> 
			& Kevin Suresh <a href="https://www.linkedin.com/in/kevititussureshtennisplayer/"><img class="social" src={linkedIn} alt="LinkedIn"/></a></p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	.social {
		width: 1em;
	}

	main {
		flex: 1;
		/* display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box; */
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
