<script type="ts">
	export let projectTitle = 'Project';
	export let projectDescription = '';
	export let appLink = '';
	export let sourceCodeLink = '';
	export let imgSrc = '';
</script>

<div class="project">
	<div class="project-l">
		<div class="info">
			<h3>{projectTitle}</h3>
			<h5>{projectDescription}</h5>
		</div>
		<div class="project-link">
			<a href={appLink} target="_blank">APP</a>
			<a href={sourceCodeLink} target="_blank">Source Code</a>
		</div>
	</div>
	<div class="project-r"><img src={imgSrc} alt="" /></div>
</div>

<style>
	.project {
		padding-top: 32px;
		display: flex;
		justify-content: space-between;
		width: 100%;
	}
	.project-l,
	.project-r {
		width: 50%;
	}
	.project-l {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}
	.info h5 {
		margin-top: 16px;
	}
	.project-link {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}
</style>
