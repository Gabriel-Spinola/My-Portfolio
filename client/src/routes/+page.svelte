<script>
	import logo from '$lib/images/me.png'
	import rebot from '$lib/images/rebot.png'
	import space from '$lib/images/space.jpg'
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Portfolio Website" />
</svelte:head>

<section id="info" class="flex flex-col gap-5">
	<article id="banner" class="text-center mt-10">
		<img alt="me" src={logo} />

		<h1>
			Gabriel Spinola<br />Portfolio
		</h1>

		<h2>
			Desenvolvedor de Sistemas Web e Jogos
		</h2>
	</article>

	<article id="flex flex-row">
		<div id="about-me">
			<h2>Hi !!</h2>
			<!-- <hr> -->
			
			<p>I'm a systems Developer focused on back-end, experienced in Go, Next.js, and TypeScript for complete Web Systems. Proficient in game development using Unity, C# and C++. Communicative and well-versed in Design Patterns, Clean Code, Restful, TDD, Git, Containers, and SOLID Principles.</p>
		</div>

		<br>

		<div id="about-me-img" class="flex-1">
			<img src={rebot} alt="rebot" />
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

		<section class="project-box">
			<div id="web-projects">
				<div>
					<h1>Builder Buddy</h1>
					<p>Description</p>
					<a href="https://projectg2.vercel.app">Prod</a>
					<a href="https://github.com/Gabriel-Spinola/Project-G-Web-Org">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>PokeGelo-CLI</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/PokeGelo-CLI">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>The Universities API</h1>
					<p>Description</p>
					<a href="https://github.com/Project-G-Org/world-universities-api">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Digital portfolio used for my lecture on Senai MG CTTI.</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/My-Programming-Portfolio-Website">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Digital portfolio used for my lecture on Senai MG CTTI.</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/Web-Projects-Collection-">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>
			</div>

			<div id="plat-projects">
				<div>
					<h1>Mental Health App</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/MentalHealthApp">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Mental Health App</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/Treino-Olimpiadas-Flutter">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>
			</div>

			<div id="games-projects">
				<div>
					<h1>Re-Bot</h1>
					<p>Description</p>
					<a href="https://github.com/Jogos-Bao-Demais/ReBot-GameJaaj6">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Hell End</h1>
					<p>Description</p>
					<a href="https://github.com/Jogos-Bao-Demais/HellEnd-VacaJam">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Uma Luz no Escuro</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/UmaLuzNoEscuro">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Parkour FPS Controller</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/Parkour-FPS-Controller-Unity">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>

				<div>
					<h1>Jumbubble</h1>
					<p>Description</p>
					<a href="https://github.com/Gabriel-Spinola/Jumbbubble-MiniJam84">Repo</a>

					Tec
					<ul>
						<li></li>
					</ul>
				</div>
			</div>

			<div id="tools-projects">

			</div>
		</section>
	</article>
	
</section>

<style>
	section {
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		font-size: 42px;
		width: 100%;
	}

	h2 {
		font-size: 22px;
		font-weight: bold;
		color: #ff77a8;
	}

	div#about-me > p {
		font-size: 18px;
		font-weight: 500;
	}

	section#info {
		background-color: #11132273;
		border-radius: 12px;
		padding: 1vw;
		border-color: #5E5E69;
		border-width: .8px;
	}

	#projects-selector ul {
		display: flex;
		flex-direction: row;
	}

	#projects-selector ul > li {
		padding: .5vw 2vw;
		font-size: 18px;
		text-decoration: dashed !important;
	}

	#projects-selector ul > li > a:hover {
		text-decoration: dashed !important;
	}
</style>
