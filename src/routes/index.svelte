<script>
 
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

.gallery{
	display: grid;
grid-template-columns: 1fr;
grid-template-rows: repeat(5, 1fr);
grid-column-gap: 0px;
grid-row-gap: 16px; 
}

.item{
	background-color: tomato;
}



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

<p>Nilson Gaspar - Product Designer. I enjoy solving problems through experimentation, compassion and a sense of humor.

	I've been a Product Designer for a few years now.<br> Right now, I'm focused on how you can save money and resources with predictive maintenance and machine learning at Jungle.ai.
	
	Before all this, I led Design at Comparamais, and before that I was part of Aptoide's design crew.
	
	<br>I grew up in Lisbon South Bay, make a lot of self deprecating jokes, and I'm notorious for being below average at singing. My hobbies range from reading about Design psychology, comic books and illustration.</p>

<figure>
	<img alt='Success Kid' src='successkid.jpg'>
	<figcaption>Have fun with Sapper!</figcaption>
</figure>

<p><strong>Try editing this file (src/routes/index.svelte) to test live reloading.</strong></p>

<div class="gallery">
	<div class="item">
		<img alt='Success Kid' src='successkid.jpg'>
	</div>
	<div class="item">
		<img alt='Success Kid' src='successkid.jpg'>
	</div>
	<div class="item"></div>
	<div class="item"></div>
</div>