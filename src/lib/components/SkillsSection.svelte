<script>
	const skillCategories = [
		{
			category: 'Frontend',
			skills: ['SvelteKit', 'TypeScript', 'JavaScript (ES6+)', 'HTML5', 'CSS3', 'Tailwind CSS']
		},
		{
			category: 'Data & State',
			skills: ['Dexie.js (IndexedDB)', 'Supabase', 'Real-time Sync']
		},
		{
			category: 'Tools & DevOps',
			skills: ['Git', 'GitHub', 'Vercel', 'VS Code', 'Linear']
		},
		{
			category: 'Libraries & Platforms',
			skills: ['D3.js', 'Capacitor', 'Tauri', 'Figma']
		}
	];
</script>

<section id="skills" class="skills-section">
	<h2 class="title">Skills<span class="accent">.</span></h2>

	<div class="skills-grid">
		{#each skillCategories as category}
			<div class="skill-category">
				<h3 class="category-title">{category.category}</h3>
				<div class="skills-list">
					{#each category.skills as skill}
						<span class="skill-tag">{skill}</span>
					{/each}
				</div>
			</div>
		{/each}
	</div>
</section>

<style>
	.skills-section {
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

	.skills-grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
		gap: 2rem;
		max-width: 1200px;
	}

	.skill-category {
		background-color: rgba(255, 255, 255, 0.03);
		border: 1px solid rgba(255, 255, 255, 0.1);
		border-radius: 8px;
		padding: 1.5rem;
		transition: border-color 0.3s ease;
	}

	.skill-category:hover {
		border-color: #00e0b8;
	}

	.category-title {
		color: #00e0b8;
		font-size: 1.1rem;
		font-weight: 600;
		margin-bottom: 1rem;
	}

	.skills-list {
		display: flex;
		flex-wrap: wrap;
		gap: 0.5rem;
	}

	.skill-tag {
		background-color: rgba(255, 255, 255, 0.05);
		border: 1px solid rgba(255, 255, 255, 0.1);
		padding: 0.4rem 0.8rem;
		border-radius: 4px;
		font-size: 0.875rem;
		color: #e5e7eb;
		transition: background-color 0.2s, border-color 0.2s;
	}

	.skill-tag:hover {
		background-color: rgba(0, 224, 184, 0.1);
		border-color: #00e0b8;
	}

	@media (max-width: 768px) {
		.skills-section {
			padding: 3rem 1.5rem;
		}

		.title {
			font-size: 2rem;
		}

		.skills-grid {
			grid-template-columns: 1fr;
			gap: 1.5rem;
		}

		.skill-category {
			padding: 1.25rem;
		}
	}
</style>
