<script lang="ts">
	let isOpen = false;
	const toggleMenu = () => (isOpen = !isOpen);
	const closeMenu = () => (isOpen = false);
</script>

<nav class="navbar">
	<div class="logo">Manoah<span>/</span></div>

	<!-- Toggle Button (Hamburger) -->
	{#if !isOpen}
		<div class="hamburger" on:click={toggleMenu}>
			<div></div>
			<div></div>
			<div></div>
		</div>
	{:else}
		<!-- Dropdown links positioned top-right where hamburger was -->
		<ul class="nav-links mobile">
			<li><a href="#about" on:click={closeMenu}>About</a></li>
			<li><a href="#experience" on:click={closeMenu}>Experience</a></li>
			<li><a href="#projects" on:click={closeMenu}>Projects</a></li>
			<li><a href="#contact" on:click={closeMenu}>Contact</a></li>
		</ul>
	{/if}

	<!-- Desktop nav -->
	<ul class="nav-links desktop">
		<li><a href="#about" class="active">About</a></li>
		<li><a href="#experience">Experience</a></li>
		<li><a href="#projects">Projects</a></li>
		<li><a href="#contact">Contact</a></li>
	</ul>
</nav>

<style>
	.navbar {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1.5rem 2rem;
		background-color: #0d1117;
		position: relative;
		z-index: 100;
	}

	/* Logo */
	.logo {
		font-size: 1.5rem;
		font-weight: bold;
		color: #fff;
	}
	.logo span {
		color: #00e0b8;
	}

	/* Hamburger icon */
	.hamburger {
		display: none;
		flex-direction: column;
		justify-content: space-between;
		width: 24px;
		height: 18px;
		cursor: pointer;
	}
	.hamburger div {
		height: 3px;
		background-color: white;
		border-radius: 1px;
	}

	/* Desktop links */
	.nav-links.desktop {
		display: flex;
		gap: 2rem;
		list-style: none;
	}
	.nav-links.desktop a {
		text-decoration: none;
		color: #c9d1d9;
		position: relative;
		padding-bottom: 4px;
		transition: color 0.2s ease;
	}
	.nav-links.desktop .active::after {
		content: '';
		position: absolute;
		left: 0;
		bottom: 0;
		width: 100%;
		height: 2px;
		background-color: #00e0b8;
	}

	/* Mobile links (dropdown) */
	.nav-links.mobile {
		top: 1.5rem;
		right: 2rem;
		background-color: #0d1117;
		border: 1px solid #222;
		border-radius: 0.375rem;
		box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
		padding: 0.5rem 1rem;
		list-style: none;
		display: flex;
		flex-direction: column;
		z-index: 200;
	}
	.nav-links.mobile li {
		margin: 0.25rem 0;
	}
	.nav-links.mobile a {
		color: #c9d1d9;
		text-decoration: none;
		transition: color 0.2s ease;
	}
	.nav-links.mobile a:hover {
		color: #00e0b8;
	}

	/* Responsive */
	@media (max-width: 768px) {
		.hamburger {
			display: flex;
		}
		.nav-links.desktop {
			display: none;
		}
	}
</style>
