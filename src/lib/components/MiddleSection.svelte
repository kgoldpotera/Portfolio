<section class="hero">
	<div class="hero-left">
		<div class="code-box">
			<img class="my-img" src="/Manoah.jpg" alt="Manoah Kipngeno" />
			<span class="code-icon">&lt;/&gt;</span>
		</div>
	</div>
	<div class="hero-right">
		<h1>
			Hi, I'm <span class="name">Manoah Kipngeno<span class="accent">.</span></span><br />
			<span class="title">Frontend Developer</span>
		</h1>
		<p class="location">Nairobi, Kenya</p>
		<div class="icons">
			<img src="/html-5-logo.svg" alt="HTML5" />
			<img src="/css-3-logo.svg" alt="CSS3" />
			<img src="/javascript-logo.svg" alt="JavaScript" />
		</div>
	</div>
</section>

<style>
	.hero {
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 4rem 2rem;
		background-color: #0d1117;
		color: #fff;
		gap: 3rem;
		flex-wrap: wrap;
	}

	@media (max-width: 768px) {
		.hero {
			padding: 2rem 1rem;
			gap: 2rem;
			flex-direction: column;
		}
	}

	.hero-left .code-box {
		width: 150px;
		height: 150px;
		border: 2px solid #00e0b8;
		position: relative;
		display: flex;
		align-items: flex-end;
		justify-content: center;
		border-radius: 4px;
	}

	.code-icon {
		position: absolute;
		bottom: -1.5rem;
		font-size: 2rem;
		color: #00e0b8;
		background-color: #0d1117;
		padding: 0 0.5rem;
	}

	.hero-right h1 {
		font-size: 2.5rem;
		line-height: 1.3;
		margin: 0;
	}

	@media (max-width: 768px) {
		.hero-right h1 {
			font-size: 1.75rem;
			text-align: center;
		}
	}

	.name {
		font-weight: bold;
	}

	.accent {
		color: #00e0b8;
	}

	.title {
		color: #94a3b8;
		font-weight: 600;
	}

	.icons {
		margin-top: 1.5rem;
		display: flex;
		gap: 1rem;
		align-items: center;
	}

	.icons img {
		width: 32px;
		height: 32px;
	}

	.my-img {
		width: 150px;
		height: 150px;
		border-radius: 4px;
	}

	.location {
		color: #94a3b8;
		margin-top: 0.5rem;
		font-size: 1rem;
	}

	@media (max-width: 768px) {
		.location {
			text-align: center;
		}

		.icons {
			justify-content: center;
		}
	}
</style>
