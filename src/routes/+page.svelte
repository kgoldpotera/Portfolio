<script>
	import Navbar from '$lib/components/Navbar.svelte';
	import MiddleSection from '$lib/components/MiddleSection.svelte';
	import TagMarquee from '$lib/components/TagMarquee.svelte';
	import AboutSection from '$lib/components/AboutSection.svelte';
	import SkillsSection from '$lib/components/SkillsSection.svelte';
	import ExperienceSection from '$lib/components/ExperienceSection.svelte';
	import ProjectSection from '$lib/components/ProjectSection.svelte';
	import ContactSection from '$lib/components/ContactSection.svelte';
</script>

<svelte:head>
	<title>Manoah Kipngeno | Frontend Developer</title>
	<meta name="description" content="Frontend Developer specializing in SvelteKit, TypeScript, and Tailwind CSS. Building production-grade applications in Nairobi, Kenya." />
</svelte:head>

<Navbar />
<MiddleSection />
<TagMarquee />
<AboutSection />
<SkillsSection />
<ExperienceSection />
<ProjectSection />
<ContactSection />
