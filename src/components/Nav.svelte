<script>
	export let segment;
	let dark = false;
	const toggleTheme = () => dark = dark === false
</script>

<style>
	nav {
		/*border-bottom: 1px solid rgba(255,62,0,0.1);*/
		font-weight: 300;
		font-size: 1.5rem;
		padding-right: 5vw;
		padding-left: 5vw;
	}

	ul {
		margin: 0;
		padding: 0;
		font-size: 1rem;
		font-family: 'Poppins', sans-serif;
		font-weight: 300;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 6px;
		background-color: rgb(255, 62, 0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}

	/* custom css starts here*/

	.toggle-dark-light {
		background-color: transparent;
		color: var(--color-text);
		border: none;

	}

	nav ul {
		width: 80%;
		display: flex;
		justify-content: flex-end;
	}

	nav .nav--logo {
		display: flex;
		justify-content: flex-start;
		width: 20%;
		font-size: 1.5rem;
		font-family: 'Poppins', sans-serif;
		font-weight: 600;
	}


















	
</style>

<svelte:head>
	{#if dark}
	<link rel="stylesheet" href="./dark-theme.css">
	{/if}
</svelte:head>

<nav>
	<a href="/" class="nav--logo">

		Nilson Gaspar
	</a>
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">Portfolio</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">Reading</a></li>

		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
		<li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="blog">Writing</a></li>
	</ul>
	<button class="toggle-dark-light" on:click={toggleTheme}>
		{#if dark}
		<link rel="stylesheet" href="./global.css">
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
			stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
			class="feather feather-moon">
			<path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
		</svg>

		{:else}
		<link rel="stylesheet" href="./dark-theme.css">
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
			stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
			class="feather feather-sun">
			<circle cx="12" cy="12" r="5"></circle>
			<line x1="12" y1="1" x2="12" y2="3"></line>
			<line x1="12" y1="21" x2="12" y2="23"></line>
			<line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line>
			<line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line>
			<line x1="1" y1="12" x2="3" y2="12"></line>
			<line x1="21" y1="12" x2="23" y2="12"></line>
			<line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line>
			<line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line>
		</svg>

		{/if}
	</button>
</nav>