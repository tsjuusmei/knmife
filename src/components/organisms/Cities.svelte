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

  div.card {
    border-radius: 20px;
    box-shadow: var(--cardshadow);
    width: auto;
    height: auto;
    padding: 2em 0;
  }

  .card > ul {
    margin: 0;
  }

  .card > img {
    display: flex;
    margin: auto;
  }

  .aligncenter {
    align-items: center;
    text-align: center;
  }

  sub {
    font-size: var(--sub);
  }
</style>

<section>
  <div class="container">
    <h2>Steden met grote uitstoot verschillen</h2>

    <p>
      De volgende steden hebben allemaal te maken gehad met de hierboven
      aangegeven maatregelen, en hebben een grote reductie in NO<sub>2</sub>
      gehad. Om deze steden te kunnen vergelijken hebben we eerst wat data per stad
      op een rijtje gezet.
    </p>

    <ul>
      <MadridCard />
      <MilanCard />
      <LyonCard />
      <LiverpoolCard />
    </ul>

    <p>
      De 4 steden bevinden zich allemaal in een ander europees land. Hierdoor is
      het makkelijker om de invloed van maatregelen te onderzoeken, en het maakt
      de vergelijkingen begrijpelijker. Ook zijn dit allemaal westerse steden
      met een andere bevolkingsdichtheid. Dit kan ook invloed hebben met de
      uitstoot.
    </p>

    <p class="margintop">
      In de onderstaande afbeelding is een visuele weergaven te zien van de
      oppervlakte van de steden. Hierbij valt het op dat Lyon twee keer het
      aantal inwoners van Liverpool heeft, maar tegelijkertijd ook de helft van
      de oppervlakte heeft. Het is gek om te zien dat Lyon ongeveer twee keer
      het aantal inwoners van Liverpool heeft, terwijl het qua oppervlakte twee
      keer zo klein is. Hetzelfde geld voor Milaan en Lyon. Dit komt door de
      grote industrie die Milaan heeft.
    </p>

    <div class="card margintop">
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

    <p class="margintop">
      In de barchart hieronder staan de gemeten NO<sub>2</sub> waardes over de
      COVID-19 periode. De balken zijn in de kleur van correspoderende stad en
      laten de hoogste, laagste en gemiddelde NO<sub>2</sub> waarde zien. Onderin
      zie je ook de datum staan van de hoogst en laagst gemeten waarde.
    </p>

    <div class="card margintop">
      <img src="../images/no2graph.jpg" alt="" />
    </div>
  </div>
</section>
