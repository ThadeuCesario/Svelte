<script>
	import Name from './components/Name/Name.svelte'
	import ReactiveAssignments from './components/ReactiveAssignments/ReactiveAssignments.svelte'
	import ReactiveDeclarations from './components/ReactiveDeclarations/ReactiveDeclarations.svelte'
	let name = "thadeu";
</script>

<main>
	<h1>Hello {name}!</h1>
	<Name name="<strong>thadeu</strong>"/>
	<ReactiveAssignments />
	<ReactiveDeclarations />
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>