<script>
  import Header from './components/organisms/Header.svelte';
  import Intro from './components/organisms/Intro.svelte';
  import Restrictions from './components/organisms/Restrictions.svelte';
  import Cities from './components/organisms/Cities.svelte';
  import No2level from './components/organisms/No2level.svelte';
  import ActiveRestrictions from './components/organisms/ActiveRestrictions.svelte';
  import MugModels from './components/organisms/MugModels.svelte';
  import Conclusion from './components/organisms/Conclusion.svelte';
  import Footer from './components/organisms/Footer.svelte';
  import Chart from './components/organisms/Chart.svelte'
</script>

<Header />
<main>
  <Intro />
  <Restrictions />
  <Cities />
  <No2level />
  <ActiveRestrictions />
  <Conclusion />
  <MugModels />
  <Footer />
  <Chart />
</main>
