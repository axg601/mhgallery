<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/sfu-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
	<div class="corner">
		<a href="https://kit.svelte.dev">
			<img src={logo} alt="SvelteKit" />
		</a>
	</div>

	<nav style="width: 100%;">
		<div style="padding-top: 2rem; width: 100%">
			<h1>
				WRIT-102: WRITING ABOUT MEDICINE
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
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		background-color: rgb(165, 11, 0);
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
	
	nav a {
		/* display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear; */
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
		--background: rgba(255, 255, 255, 0.7);
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

</style>
