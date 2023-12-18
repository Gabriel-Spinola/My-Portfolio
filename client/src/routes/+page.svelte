<script>
	import logo from '$lib/images/me.png'
	import rebot from '$lib/images/rebot.png'
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Portfolio Website" />
</svelte:head>

<section class="flex flex-col gap-5">
	<article id="banner" class="text-center mt-10">
		<img alt="me" src={logo} />

		<h1>
			Gabriel Spibola<br />Portfolio
		</h1>

		<h2>
			Desenvolvedor de Sistemas Web e Jogos
		</h2>
	</article>

	<article id="flex flex-row">
		<div id="about-me">
			<h2>Hi!</h2>
			<p>Systems Developer focused on back-end, experienced in PHP, HTML, CSS, JS, Next.js, and TypeScript for complete Web Systems. Proficient in game development using Unity and C#. Communicative and well-versed in Design Patterns, Clean Code, Restful, TDD, Git, Containers, and SOLID Principles.</p>
		</div>

		<div id="about-me-img" class="flex-1">
			<img src={rebot} />
		</div>
	</article>

	<article id="projects">
		<nav id="projects-selector" class="flex flex-row">
			<ul class="text-white">
				<li><a href="#web">Web Projects</a></li>
				<li><a href="#plat">Desktop/Mobile Projects</a></li>
				<li><a href="#tools">Tools</a></li>
				<li><a href="#games">Games</a></li>
			</ul>
		</nav>

		<div class="project-box">

		</div>
	</article>
	
</section>

<style>
	section {
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		font-size: xx-large;
		width: 100%;
	}
</style>
