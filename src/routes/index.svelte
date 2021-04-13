<script>
 import Gallery from 'svelte-image-gallery'
</script>


<style>
	/* h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	} */

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
	}


	.big-title {
		font-size: 4rem;
		font-family: 'Merriweather', serif;
	}









/* mansory articles gallery*/
:global(img) { opacity: .9; transition: all .2s }
:global(img):hover { opacity: 1; transform: scale(1.04) }









	@media (min-width: 480px) {
		p {
			font-size: 1.4rem;
			
			
		font-weight: 300;
		margin: 0 0 0.5em 0;
		}
	}



</style>

<svelte:head>
	<title>Nilson Gaspar</title>
	
</svelte:head>

<p> 
	<span class="big-title">I'm Nilson Gaspar.</span>
</p>
<p>Senior designer at <a href="https://ki-challengers.com/">KI Challenge.rs</a>. I'm a human centered Design practitioner, who enjoys solving problems through experimentation, compassion and a sense of humor. </p>

<figure>
	<img alt='Success Kid' src='successkid.jpg'>
	<figcaption>Have fun with Sapper!</figcaption>
</figure>

<p><strong>Try editing this file (src/routes/index.svelte) to test live reloading.</strong></p>

<Gallery gap="10" maxColumnWidth="200">
	<img src="https://via.placeholder.com/180x200/1" alt="">
	<img src="https://via.placeholder.com/200x280/1" alt="">
	<img src="https://via.placeholder.com/250x200/1" alt="">
	<img src="https://via.placeholder.com/140x310/1" alt="">
	<!-- <img src="https://via.placeholder.com/280x300/1" alt="">
	<img src="https://via.placeholder.com/220x100/1" alt="">
	<img src="https://via.placeholder.com/180x150/1" alt="">
	<img src="https://via.placeholder.com/210x180/1" alt="">
	<img src="https://via.placeholder.com/210x200/1" alt=""> -->
	
</Gallery>