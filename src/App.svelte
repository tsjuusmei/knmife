<script>
	import Header from "./components/organisms/Header.svelte";
	import Intro from "./components/organisms/Intro.svelte";
	import Maatregelen from "./components/organisms/Maatregelen.svelte"
	import Steden from "./components/organisms/Steden.svelte"
</script>

<body>
	<Header />
	<Intro />
	<Maatregelen />
	<Steden />
</body>

<style>
	body {
		overflow-x: hidden;
		scroll-behavior: smooth;
	}
</style>