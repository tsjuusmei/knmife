<script>
	import Header from "./components/organisms/Header.svelte";
	import Intro from "./components/organisms/Intro.svelte";
	import Maatregelen from "./components/organisms/Maatregelen.svelte"
</script>

<body>
	<Header />
	<Intro />
	<Maatregelen />
</body>

<style>
	body {
		overflow-x: hidden;
		scroll-behavior: smooth;
	}
</style>