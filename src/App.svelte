<script>
	import Header from './components/Header.svelte';
	import Anime from './components/Anime.svelte';
	import Footer from './components/Footer.svelte';
	import Tabs from './shared/Tabs.svelte';
	import Button from './shared/Button.svelte';
	import Card from './shared/Card.svelte';
	import { navOptions } from './components/Nav.svelte';

	let selected = navOptions[0];	
	let intSelected = 0;	
	
	function changeComponent(event) {
		selected = navOptions[event.srcElement.id];
		intSelected = event.srcElement.id;
	}
</script>
	
<link rel='stylesheet' href='https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css'>
<Header />
<Anime />
<br>
<div class="container">
	<ul class="nav nav-tabs loco">
		{#each navOptions as option, i}
		<li class="nav-item">
			<button class={intSelected==i ? "nav-link active p-2 ml-1" : "p-2 ml-1 nav-link"} on:click={changeComponent} id={i} role="tab">{option.page}</button>
		</li>
		{/each}
	</ul>	
	<div class="row">
		<div class="col-sm-12">
			<div class="p-2">
				<svelte:component this={selected.component}/>
			</div>
		</div>
	</div>	
</div>
<Footer />


<style>
	@import url('https://fonts.googleapis.com/css2?family=Boogaloo&display=swap');
	
	.loco {
		margin-top: 40px;
		font-family: 'Share Tech Mono', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif;
		font-size: 27px;
		text-decoration: none;
	}
</style>	 	
