<script>
	import Nav from '../components/Nav.svelte';
	import Project from '../components/Project.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		
		
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
	<Project/>
</main>