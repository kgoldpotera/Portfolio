<script>
</script>

<section id="experience" class="experience-section">
	<h2 class="title">Experience<span class="accent">.</span></h2>

	<div class="experience-item">
		<p class="duration">May 2025 – July 2025</p>
		<h3 class="role">Frontend Developer Intern | Drug Index (HealthTech Startup)</h3>
		<p class="description">
			Built the <strong>Brand PriceChart module</strong> using SvelteKit and D3.js, creating interactive line graphs to visualize historical drug pricing trends. Configured and managed build pipelines for <strong>Tauri (Windows/macOS)</strong> and <strong>Capacitor (Android/iOS)</strong> for native deployment.
		</p>
		<p class="description">
			Enhanced platform <strong>accessibility</strong> with ARIA labels and keyboard navigation. Standardized design system by implementing unified button classes and refactoring Admin Sidebar to match modern UI aesthetics.
		</p>
		<p class="description">
			Conducted rigorous QA testing using Linear for issue tracking, resolving bugs related to session management, light/dark mode, and mobile responsiveness.
		</p>
	</div>

	<div class="experience-item">
		<p class="duration">Jan 2024 – Present</p>
		<h3 class="role">Freelance Web Developer</h3>
		<p class="description">
			Developed custom, responsive websites for clients using HTML, CSS, and JavaScript, ensuring 100% mobile compatibility. Translated client requirements into functional user interfaces with fast load times and SEO best practices.
		</p>
		<p class="description">
			Managed deployment and hosting configurations to ensure high uptime for client portfolios.
		</p>
	</div>
</section>

<style>
	.experience-section {
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

	.experience-item {
		margin-bottom: 2.5rem;
	}

	.duration {
		color: #00e0b8;
		font-weight: 500;
		margin-bottom: 0.25rem;
	}

	.role {
		font-size: 1.2rem;
		color: #ffffff;
		font-weight: 600;
		margin-bottom: 0.5rem;
		display: flex;
		align-items: center;
		gap: 0.25rem;
	}

	.description {
		color: #c9d1d9;
		line-height: 1.6;
		max-width: 800px;
		margin-bottom: 0.5rem;
	}

	@media (max-width: 768px) {
		.experience-section {
			padding: 3rem 1.5rem;
		}

		.title {
			font-size: 2rem;
		}

		.role {
			font-size: 1.1rem;
			flex-wrap: wrap;
		}

		.description {
			font-size: 0.95rem;
		}
	}
</style>
