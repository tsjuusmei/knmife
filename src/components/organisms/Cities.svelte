<script>
  import MadridCard from '../molecules/MadridCard.svelte';
  import MilanCard from '../molecules/MilanCard.svelte';
  import LyonCard from '../molecules/LyonCard.svelte';
  import LiverpoolCard from '../molecules/LiverpoolCard.svelte';
  import MadridSurface from '../molecules/MadridSurface.svelte';
  import MilanSurface from '../molecules/MilanSurface.svelte';
  import LyonSurface from '../molecules/LyonSurface.svelte';
  import LiverpoolSurface from '../molecules/LiverpoolSurface.svelte';
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
    margin: 110px 0;
    justify-content: space-evenly;
    padding: 0;
  }

  .margintop {
    margin-top: 4em;
  }

  div.surfaces {
    border-radius: 20px;
    box-shadow: var(--cardshadow);
    width: 100%;
    height: 60vh;
  }

  .aligncenter {
    align-items: center;
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
      <LiverpoolCard />
    </ul>

    <p>
      Zoals te zien is hebben we gekozen voor 4 steden die zich allemaal in een
      ander europees land bevinden. Dit hebben wij gedaan om te kunnen
      vergelijken of maatregelen in een andere stad met meer of minder
      bevolkingsdichtheid verschil maakt.
    </p>

    <p class="margintop">
      In de onderstaande afbeelding is een visuele weergaven te zien van de 4
      gekozen steden in vierkante kilometer. Het is gek om te zien dat Lyon
      ongeveer twee keer het aantal inwoners van Liverpool heeft, terwijl het
      qua oppervlakte twee keer zo klein is.
    </p>

    <div class="surfaces margintop">
      <ul class="aligncenter">
        <li>
          <MadridSurface />
        </li>
        <li>
          <MilanSurface />
        </li>
        <li>
          <LyonSurface />
        </li>
        <li>
          <LiverpoolSurface />
        </li>
      </ul>
    </div>
  </div>
</section>
