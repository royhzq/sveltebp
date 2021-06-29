<script>
	import { Router, Route } from "svelte-routing";
	import Header from './components/Header.svelte';
	import About from './routes/About.svelte';
	import Home from './routes/Home.svelte';

	let name = 'world';
	export let url ="";

</script>

<Header />
<Router url="{url}">
	<div>
	  <Route path="/"><Home /></Route>
	  <Route path="about"><About /></Route>
	</div>
</Router>
