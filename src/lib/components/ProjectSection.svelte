<script>
	// Optional: Can later use an array of project objects
</script>

<section id="projects" class="project-section">
	<h2 class="title">Projects<span class="accent">.</span></h2>

	<div class="project-item">
		<h3 class="project-title">
			Awesome Portfolio <a href="#" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">Svelte • Tailwind • TypeScript</p>
		<p class="description">
			A responsive portfolio website showcasing developer skills and projects. Built with SvelteKit
			and styled using Tailwind CSS. It supports smooth scroll navigation and reusable components.
		</p>
	</div>

	<div class="project-item">
		<h3 class="project-title">
			Task Manager App <a href="#" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">React • Firebase • CSS Modules</p>
		<p class="description">
			A simple productivity web app allowing users to manage tasks and set reminders. Features user
			authentication, real-time syncing with Firebase, and a clean UI.
		</p>
	</div>

	<div class="project-item">
		<h3 class="project-title">
			Markdown Blog Engine <a href="#" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">Node.js • Express • EJS</p>
		<p class="description">
			A minimal blog engine built with Node.js and Express. Supports markdown rendering, blog post
			routing, and dynamic content updates with EJS templating.
		</p>
	</div>
</section>

<style>
	.project-section {
		padding: 4rem 2rem;
		background-color: #0d1117;
		color: #c9d1d9;
	}

	.title {
		font-size: 2.5rem;
		font-weight: 800;
		color: #fff;
		margin-bottom: 2rem;
	}

	.accent {
		color: #00e0b8;
	}

	.project-item {
		margin-bottom: 2.5rem;
	}

	.project-title {
		font-size: 1.2rem;
		color: #ffffff;
		font-weight: 600;
		margin-bottom: 0.25rem;
		display: flex;
		align-items: center;
		gap: 0.25rem;
	}

	.project-title a {
		color: #00e0b8;
		text-decoration: none;
		font-size: 1rem;
	}

	.tech-stack {
		color: #00e0b8;
		font-weight: 500;
		margin-bottom: 0.5rem;
	}

	.description {
		color: #c9d1d9;
		line-height: 1.6;
		max-width: 800px;
	}
</style>
