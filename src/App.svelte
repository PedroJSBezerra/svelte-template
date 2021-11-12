<script lang="ts">
	import Router from 'svelte-spa-router'
	import Home from './routes/Home.svelte'
	import Contact from './routes/Contact.svelte'
	
	let routes = {
		'/': Home,
		'/contact': Contact
	}

	let svelte: string
	let typescript: string
	let sass: string

	svelte = 'Svelte'
	typescript = 'Typescript'
	sass = 'Sass'
</script>

<div class="app">
	<nav>
		<a href="/#/">Home</a>
		<a href="/#/contact">Contact</a>
	</nav>

	<Router {routes} />
</div>