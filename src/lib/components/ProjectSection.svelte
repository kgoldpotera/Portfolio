<script>
</script>

<section id="projects" class="project-section">
	<h2 class="title">Projects<span class="accent">.</span></h2>

	<div class="project-item">
		<h3 class="project-title">
			Komuche (Kenyan Style) <a href="https://komuche-kenyan-style.vercel.app/" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">SvelteKit • Tailwind CSS • AI Integration • Vercel</p>
		<p class="description">
			AI-powered e-commerce platform tailored for the Kenyan fashion market with responsive mobile design. Engineered a built-in <strong>Virtual Stylist</strong> feature utilizing AI to provide real-time, personalized outfit recommendations. Implemented seamless shopping experience with optimized product filtering and fast page loads.
		</p>
	</div>

	<div class="project-item">
		<h3 class="project-title">
			Dynamic Weather App <a href="https://my-weather-app-zeta-three.vercel.app/" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">JavaScript • REST API • CSS</p>
		<p class="description">
			Location-based weather application that fetches real-time meteorological data via API. Implemented <strong>conditional UI logic</strong> to dynamically change background theme based on user's location and current weather conditions. Demonstrated mastery of asynchronous JavaScript (Promises/Async-Await) and DOM manipulation.
		</p>
	</div>

	<div class="project-item">
		<h3 class="project-title">
			Personal Portfolio <a href="https://myportfolio-six-taupe-30.vercel.app/" target="_blank" rel="noopener noreferrer">↗</a>
		</h3>
		<p class="tech-stack">SvelteKit • Vercel • CSS</p>
		<p class="description">
			Designed and deployed a personal portfolio to showcase development skills and case studies. Implemented clean, component-driven architecture to demonstrate mastery of SvelteKit routing and layout systems.
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

	@media (max-width: 768px) {
		.project-section {
			padding: 3rem 1.5rem;
		}

		.title {
			font-size: 2rem;
		}

		.project-title {
			font-size: 1.1rem;
			flex-wrap: wrap;
		}

		.description {
			font-size: 0.95rem;
		}
	}
</style>
