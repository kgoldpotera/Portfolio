<script>
	const contacts = [
		{
			label: 'Linkedin',
			icon: '/linkedin-logo.svg',
			href: 'https://www.linkedin.com/in/manoah-koech-76a25b249',
			newTab: true
		},
		{
			label: 'GitHub',
			icon: '/github.svg',
			href: 'https://github.com/kgoldpotera',
			newTab: true
		},
		{
			label: 'E-mail',
			icon: '/gmail.svg',
			href: 'mailto:koechmanoah32@gmail.com',
			newTab: false
		}
	];
</script>

<section id="contact" class="contact-section">
	<h2 class="title">Contact<span class="accent">.</span></h2>
	<p class="subtitle">Contact me or follow my social media</p>

	<div class="grid">
		{#each contacts as contact (contact.label)}
			<a
				class="card"
				href={contact.href}
				target={contact.newTab ? '_blank' : '_self'}
				rel={contact.newTab ? 'noopener noreferrer' : ''}
			>
				<div class="card-left">
					<img src={contact.icon} alt={contact.label + ' icon'} class="icon" />
					<span>{contact.label}</span>
				</div>
				<span class="arrow">↗</span>
			</a>
		{/each}
	</div>
</section>

<style>
	.contact-section {
		padding: 4rem 2rem;
		background-color: #0d1117;
		color: #c9d1d9;
		text-align: center;
	}

	.title {
		font-size: 2.5rem;
		font-weight: 800;
		color: #fff;
		margin-bottom: 0.5rem;
	}

	.accent {
		color: #00e0b8;
	}

	.subtitle {
		margin-bottom: 2rem;
		color: #94a3b8;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
		gap: 1rem;
		justify-items: center;
		max-width: 800px;
		margin: 0 auto;
	}

	.card {
		display: flex;
		justify-content: space-between;
		align-items: center;
		width: 100%;
		padding: 4px;
		background-color: #111827;
		border: 1px solid #1f2937;
		border-radius: 8px;
		text-decoration: none;
		color: #fff;
		transition: border 0.2s ease;
	}

	.card:hover {
		border-color: #00e0b8;
	}

	.card-left {
		display: flex;
		align-items: center;
		gap: 0.75rem;
		font-weight: 600;
	}

	.icon {
		width: 20px;
		height: 20px;
		object-fit: contain;
	}

	.arrow {
		color: #00e0b8;
		font-size: 1rem;
	}
</style>
