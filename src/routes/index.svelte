

<script>
	import films from '$lib/listing.js'
	/*const priceTTC = (price) => price * 1.2*/

</script>


<section>
	{#each films as film}
		<div class="titre">{film.titre} <!--price : {priceTTC(product.price)}--></div>
		<div class="infos"><div class="categ">Date de sortie:</div>{film.date} </div>
		<div class="infos"><div class="categ">Réalisateur:</div>{film.real} </div>
		<div class="infos"><div class="categ">Durée:</div>{film.duree} </div>
		<div class="infos"><div class="categ">Genre:</div>{film.genre} </div>
		<div class="infos"><div class="categ">Note Imdb:</div>{film.imdbrating} </div>
		<div class="resume"><div class="categ">Résumé:</div>{film.pitch} </div>
	{/each}
</section>

<!--
<input id="searchbar" onkeyup="search_animal()" type="text" name="search" placeholder="Search animals..">-->
      
    <!-- ordered list 
    <ol id='list'>
        <li class="titre">Cat</li>
        <li class="animals">Dog</li>
        <li class="animals">Elephant</li>
        <li class="animals">Fish</li>
        <li class="animals">Gorilla</li>
        <li class="animals">Monkey</li>
        <li class="animals">Turtle</li>
        <li class="animals">Whale</li>
        <li class="animals">Aligator</li>
        <li class="animals">Donkey</li>
        <li class="animals">Horse</li>
    </ol>

		      
     linking javascript 
    <script src="./listing.js"></script>-->


<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	.titre{
		border: solid 0px black;
		width: 100%;
		color: #C60800;
		font-weight: bold;
		font-size: 30;
		padding: 20px 50px 8px;
		
	}

	.infos{
		border: solid 0px black;
		width: 100%;
		padding: 8px 8px;
		margin-left: 60%;
	}

	.resume{
		border: solid 0px black;
		width: 100%;
		padding: 8px 8px;
		margin-left: 0%;
	}

	.categ{
		border: solid 0px black;
		width: 100%;
		font-weight: bold;
		
	}


</style>
