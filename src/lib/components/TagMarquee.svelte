<script>
	export let tags = [
		'SVELTEKIT',
		'TYPESCRIPT',
		'TAILWIND CSS',
		'JAVASCRIPT',
		'HTML5',
		'CSS3',
		'FIGMA',
		'GIT',
		'DEXIE.JS',
		'SUPABASE',
		'D3.JS',
		'CAPACITOR',
		'TAURI',
		'RESPONSIVE DESIGN'
	];
</script>

<section class="tag-marquee">
	<div class="tag-track">
		<div class="tag-list">
			{#each tags as tag, i (tag)}
				<div class="tag">{tag}</div>
			{/each}
		</div>
		<div class="tag-list">
			{#each tags as tag, i (tag + '-copy')}
				<div class="tag">{tag}</div>
			{/each}
		</div>
	</div>
</section>

<style>
	.tag-marquee {
		background-color: rgba(13, 17, 23, 0.6);
		backdrop-filter: blur(12px);
		-webkit-backdrop-filter: blur(12px);
		border-top: 1px solid rgba(255, 255, 255, 0.08);
		border-bottom: 1px solid rgba(255, 255, 255, 0.08);
		padding: 1rem 0;
		overflow: hidden;
		position: relative;
	}

	.tag-track {
		display: flex;
		width: max-content;
		animation: scroll-left 40s linear infinite;
	}

	@keyframes scroll-left {
		from {
			transform: translateX(0%);
		}
		to {
			transform: translateX(-50%);
		}
	}

	.tag-list {
		display: flex;
		gap: 1rem;
		padding: 0 2rem;
	}

	.tag {
		background: rgba(255, 255, 255, 0.05);
		border: 1px solid rgba(255, 255, 255, 0.1);
		backdrop-filter: blur(6px);
		-webkit-backdrop-filter: blur(6px);
		padding: 0.5rem 1rem;
		border-radius: 9999px;
		font-weight: 600;
		font-size: 0.875rem;
		color: #e5e7eb;
		text-transform: uppercase;
		white-space: nowrap;
		transition: background 0.3s, color 0.3s;
	}

	.tag:hover {
		background: rgba(0, 224, 184, 0.1);
		color: #00e0b8;
		cursor: pointer;
	}

	@media (max-width: 768px) {
		.tag-marquee {
			padding: 0.75rem 0;
		}

		.tag {
			padding: 0.4rem 0.8rem;
			font-size: 0.75rem;
		}

		.tag-list {
			gap: 0.75rem;
			padding: 0 1rem;
		}
	}
</style>
