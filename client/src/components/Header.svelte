<script>
	import { page } from '$app/stores';
	
	import github from '$lib/images/github.svg';
	import itchio from '$lib/images/itch-io.svg'
	import twitter from '$lib/images/twitter.svg';
	import gmail from '$lib/images/envelope-solid.svg';
	import linkedin from '$lib/images/linkedin.svg'
</script>

<header>
	<nav class="width-full flex flex-row text-center items-center p-7">
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>

		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>

			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
		</ul>
		
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<div class="corner align-middle mt-6 mr-8">
		<a href="https://github.com/Gabriel-Spinola">
			<img src={github} alt="GitHub" />
		</a>

		<a href="https://gabriel-spinola.itch.io">
			<img id="itch-icon" src={itchio} alt="itch.io">
		</a>

		<a href="mailto:gabrielspinola77@gmail.com">
			<img id="itch-icon" src={gmail} alt="gmail">
		</a>
		
		<a href="https://twitter.com/gabrielsevin7">
			<img id="itch-icon" src={twitter} alt="twitter">
		</a>

		<a href="https://www.linkedin.com/in/gabriel-spinola-b64b5b273/">
			<img id="itch-icon" src={linkedin} alt="twitter">
		</a>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		background-color: #ff77a8;
		border-color: #ffec27;
		border-width: 1px;
		border-top: none;
		border-left: none;
		border-right: none;
	}

	.corner {
		width: 10em;
		height: 3em;
		display: flex;
		flex-direction: row;
		gap: 1vw;
		margin-right: 8vw;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
		font-size: 1.4rem;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
		margin: 1vw;
	}

	#itch-icon {
		width: 80%;
		height: 80%;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: #14182e;
	}

	nav li a {
		color: white;
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

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.94rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
