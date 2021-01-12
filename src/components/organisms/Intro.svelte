<script>
  // import Clouds from "../molecules/Clouds.svelte";
  import Molecules from '../molecules/Molecules.svelte';
</script>

<style>
  section {
    height: 100vh;
    background-color: white;
    margin-bottom: -2%;
  }

  h2 {
    font-family: 'Sora';
    font-size: 72px;
    text-align: center;
    margin-right: 5%;
    color: var(--darkblue);
  }

  p {
    font-size: 16px;
    width: 45%;
    margin-left: 150px;
    line-height: 2em;
  }

  span {
    font-size: 0.5em;
    font-weight: 700;
  }
</style>

<section>
  <!-- <Clouds /> -->

  <div class="container">
    <Molecules />
    <h2>Wat is NO<span>2</span>?</h2>

    <p>
      De uitstoot van NO<span>2</span>
      is de afgelopen jaren veel te hoog. Door COVID-19 zijn er verschillende
      maatregelen van pas gekomen, waardoor het vervoer en producties
      verminderden. De invloed van deze maatregelen staan in dit artikel
      verwerkt. Stikstofdioxide (NO<span>2</span>) is een gas dat in Nederland
      voor een groot gedeelte door het autoverkeer wordt geproduceerd. Het is
      daarom een belangrijke indicator voor de luchtverontreiniging door
      verkeer. Langs grote wegen komen hoge concentraties voor die over een
      afstand van enkele kilometers afnemen tot lage concentraties. Bovendien
      draagt Stikstofdioxide ook bij aan smog.
    </p>
  </div>
</section>
