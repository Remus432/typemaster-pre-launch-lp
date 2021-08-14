<script>
	import Nav from "./Nav.svelte";
	import Header from "./Header.svelte";
	import Showcase from "./Showcase.svelte";
	import Features from "./Features.svelte";
</script>

<main>
	<Nav/>
	<Header/>
	<Showcase/>
	<Features/>
	<footer>
		<span>Typemaster 2021</span> &nbsp;  | &nbsp;  All Rights Reserved
	</footer>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@500;900&display=swap');

	main {
		padding: 3rem;
	}

	footer {
		text-align: center;
		color: var(--grayish-blue);
		margin-bottom: 2rem;
	}

	span {
		font-weight: bold;
	}

	@media (min-width: 1440px) {
		main {
			padding: 3rem 18rem;
		}
	}
</style>