<script>
</script>

<section id="about" class="about-section">
	<h2 class="title">About<span class="accent">.</span></h2>
	<div class="content">
		<div class="text">
			<p>
				Innovative <strong>Frontend Developer</strong> with strong expertise in <strong>SvelteKit</strong>, <strong>TypeScript</strong>, and <strong>Tailwind CSS</strong>. Proven experience building production-grade applications with offline-first capabilities and real-time data synchronization.
			</p>

			<p>
				Skilled in bridging the gap between design and development, optimizing UI performance, and configuring cross-platform builds for web, desktop (Tauri), and mobile. Passionate about creating impactful digital solutions that solve real-world problems.
			</p>

			<p>
				Currently on industrial attachment at <strong>Drug Index</strong>, where I contribute to building innovative HealthTech solutions while pursuing my degree in Telecommunication and Information Technology at Kenyatta University.
			</p>
		</div>
	</div>
</section>

<style>
	.about-section {
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

	.content {
		display: flex;
		flex-wrap: wrap;
		gap: 2rem;
		align-items: flex-start;
	}

	.text {
		flex: 1;
		max-width: 600px;
		display: flex;
		flex-direction: column;
		gap: 1rem;
		font-size: 1rem;
		line-height: 1.6;
	}

	@media (max-width: 768px) {
		.about-section {
			padding: 3rem 1.5rem;
		}

		.title {
			font-size: 2rem;
		}

		.text {
			font-size: 0.95rem;
		}
	}
</style>
