<script lang="ts">
	import Project from './Project.svelte';

	type ProjectData = {
		title: string;
		description: string;
		appLink: string;
		sourceCodeLink: string;
		imgSrc: string;
	};

	let projects = new Map<string, ProjectData>();

	projects.set('project1', {
		title: 'Project1',
		description: 'Project1 Description',
		appLink: 'https://apps.apple.com/jp/app/pair-schedule/id6448741321',
		sourceCodeLink: 'https://github.com/Muhyun-Kim/couple_share_schedule',
		imgSrc: '/images/profile.png'
	});

	let projectEntries = Array.from(projects.entries());
</script>

<div class="project-page">
	<div class="project-page-frame">
		<h1>Project</h1>
		{#each projectEntries as [key, project]}
			<Project
				projectTitle={project.title}
				projectDescription={project.description}
				appLink={project.appLink}
				sourceCodeLink={project.sourceCodeLink}
				imgSrc={project.imgSrc}
			/>
		{/each}
	</div>
</div>

<style>
	.project-page {
		display: flex;
		justify-content: center;
	}
	.project-page-frame {
		width: 80%;
	}
</style>
