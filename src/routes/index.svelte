<script>
 import Footer from '../components/Footer.svelte';
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


/* 	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}
 */
	p {
		margin: 1em auto;
	}


	.big-title {
		font-size: 4rem;
		font-family: 'Merriweather', serif;
	}



	.grid-item {
  display: flex;
  align-items: center;
  justify-content: center;

  background-color: #03afff;
  border-radius: 4px;
  transition: transform 0.3s ease-in-out;

  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.grid-item:hover {
  filter: opacity(0.9);
  transform: scale(1.04);
}

.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  grid-auto-rows: minmax(200px, auto);
  gap: 20px;
  padding: 20px;
  grid-auto-flow: dense;
}

@media (min-width: 600px) {
  .wide {
    grid-column: span 2;
  }

  .tall {
    grid-row: span 2;
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


<div class="grid-container">
	<div class="grid-item tall" style="background-image: url('https://picsum.photos/id/65/900/900.jpg')"></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/881/900/900.jpg');
		  "></div>
  
	<div class="grid-item wide" style="
			background-image: url('https://picsum.photos/id/248/900/900.jpg');
		  "></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/423/900/900.jpg');
		  "></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/534/900/900.jpg');
		  "></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/664/900/900.jpg');
		  "></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/176/900/900.jpg');
		  "></div>
	<div class="grid-item" style="background-image: url('https://picsum.photos/id/73/900/900.jpg')"></div>
	<div class="grid-item tall wide" style="
			background-image: url('https://picsum.photos/id/806/900/900.jpg');
		  "></div>
	<div class="grid-item" style="
			background-image: url('https://picsum.photos/id/535/900/900.jpg');
		  "></div>
	
	
  </div>

  <Footer/>