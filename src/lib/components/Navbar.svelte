<nav class="navbar">
	<div class="logo">Manoah<span>/</span></div>
	<ul class="nav-links">
		<li><a href="#about" class="active">About</a></li>
		<li><a href="#experience">Experience</a></li>
		<li><a href="#projects">Projects</a></li>
		<li><a href="#contact">Contact</a></li>
	</ul>
</nav>

<style>
	/* Navbar container */
	.navbar {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1.5rem 2rem;
		background-color: #0d1117;
	}

	/* Logo styling */
	.logo {
		font-size: 1.5rem;
		font-weight: bold;
		color: #fff;
	}

	.logo span {
		color: #00e0b8;
	}

	/* Nav list styling */
	.nav-links {
		list-style: none;
		display: flex;
		gap: 2.5rem;
		margin: 0;
		padding: 0;
	}

	/* Nav link styling */
	.nav-links a {
		text-decoration: none;
		color: #c9d1d9;
		position: relative;
		padding-bottom: 4px;
		transition: color 0.2s ease;
	}

	/* Hover effect */
	.nav-links a:hover {
		color: #00e0b8;
	}

	/* Active link underline */
	.nav-links .active::after {
		content: '';
		position: absolute;
		left: 0;
		bottom: 0;
		width: 100%;
		height: 2px;
		background-color: #00e0b8;
	}

	@media (max-width: 768px) {
		/* CSS rules for screens 768px wide or narrower */
		.nav-links {
			display: flex;
			flex-direction: column;
			align-items: flex-start;
		}
	}
</style>
