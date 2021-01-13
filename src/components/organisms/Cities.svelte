<script>
  import MadridCard from '../molecules/MadridCard.svelte';
  import MilanCard from '../molecules/MilanCard.svelte'
  import LyonCard from '../molecules/LyonCard.svelte'
</script>

<style>
  h3 {
    font-family: 'Sora';
    color: var(--darkblue);
    font-size: 30px;
    padding-top: 5%;
    text-align: center;
  }

  p {
    width: 55%;
    line-height: 2em;
    margin: auto;
  }

  section {
    height: 100vh;
  }

  ul {
    list-style-type: none;
    display: flex;
    margin: 110px;
    justify-content: space-between;
    padding: 0;
  }
</style>

<section>
  <div class="container">
    <h3>Welke steden hebben wij gekozen en waarom?</h3>

    <p>
      De volgende steden hebben allemaal te maken gehad met de hierboven
      aangegeven maatregelen. Om deze steden te kunnen vergelijken hebben we
      eerst wat data per stad op een rijtje gezet.
    </p>

    <ul>
      <MadridCard />
      <MilanCard />
      <LyonCard />
      <li />
    </ul>
  </div>
</section>
